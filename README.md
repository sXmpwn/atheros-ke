![atheros-kexts](https://user-images.githubusercontent.com/73723350/132765050-02e7d64f-7523-4601-a2c7-347bf4161f67.PNG)

## Supported Devices

- AR9281
- AR5418/5133
- AR9280 
- AR9380
- AR94621
- AR9283
- AR9285
- AR9287
- AR94851

## Models

Verified to work with an TP-Link TL-WN881ND (AR9287) on Big Sur and lower.

## Supported macOS versions

macOS 10.14, Mojave - macOS 10.15, Catalina and macOS 11, Big Sur

(shouldn't be needed on 10.13 unless the PCIe-ID of the chipset isn't present)

![Mojave](https://user-images.githubusercontent.com/73723350/132761272-c6419531-7a0f-4e5a-8de8-3879b7e76fb7.png) ![Catalina](https://user-images.githubusercontent.com/73723350/132761288-e9fd03c7-b40f-48d8-82ce-e0bd0f0656fd.png) ![Big Sur](https://user-images.githubusercontent.com/73723350/132761312-25d70372-b207-4296-b151-77af511273a2.png)

Monterey+ is excluded and likely won't be compatible ever.

## Installation
### OpenCore
Download those 2 Kexts from Release, "AirPortAtheros40.kext" and "HS80211Family.kext" and put these into EFI/OC/Kexts, add them into your config.plist or do an OC Snapshot if you’re using ProperTree. 

Make sure that "HS80211Family.kext" is loading first and that "AirPortAtheros40.kext" is loading after it in the config.plist. 

It should exactly look like this:

![Example](https://user-images.githubusercontent.com/73723350/131271107-abe28193-fd69-4ad6-ab0c-51a306b68928.png)

Note that this is case-sensitive, without it, it won’t work!

### Clover 
Download those 2 Kexts from Release, "AirPortAtheros40.kext" and "HS80211Family.kext" and put these into CLOVER/Kexts/Other.

## Credits

• [pico joe](https://www.insanelymac.com/forum/profile/1113740-pico-joe) for the base modifications 

• [khronokernel](https://github.com/khronokernel) for dumping High Sierra's IO80211Family
