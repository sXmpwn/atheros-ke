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

Support coming to AR9565 and AR9485 very soon

## Supported macOS versions

macOS High Sierra, macOS Mojave, macOS Catalina and macOS Big Sur

![High Sierra](https://user-images.githubusercontent.com/73723350/132761234-e861613d-de45-4184-8df3-0719bc75cbf8.png) ![Mojave](https://user-images.githubusercontent.com/73723350/132761272-c6419531-7a0f-4e5a-8de8-3879b7e76fb7.png) ![Catalina](https://user-images.githubusercontent.com/73723350/132761288-e9fd03c7-b40f-48d8-82ce-e0bd0f0656fd.png) ![Big Sur](https://user-images.githubusercontent.com/73723350/132761312-25d70372-b207-4296-b151-77af511273a2.png)

## Installation
### OpenCore
Download those 2 Kexts, "AirPortAtheros40.kext" and "HS80211Family.kext", put these into EFI/OC/Kexts, add them into your config.plist or do an OC Snapshot if you’re using ProperTree. 

Make sure that "HS80211Family.kext" is loading first and that "AirPortAtheros40.kext" is loading after it in the config.plist. 
Note that this is case-sensitive, without it, it won’t work!

It should exactly look like this:

![Example](https://user-images.githubusercontent.com/73723350/131271107-abe28193-fd69-4ad6-ab0c-51a306b68928.png)

### Clover 
Download those 2 Kexts, "AirPortAtheros40.kext" and "HS80211Family.kext", put these into CLOVER/Kexts/Other.
