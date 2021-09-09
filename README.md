![atheros-kexts](https://user-images.githubusercontent.com/73723350/131275377-7b12997a-0dd0-43a8-9ff2-13a7902a0497.png)

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
- Support coming to AR9565 and AR9485 very soon

## Installation
### OpenCore
Download those 2 Kexts, "AirPortAtheros40.kext" and "HS80211Family.kext", put these into EFI/OC/Kexts, add them into your config.plist or do an OC Snapshot if you’re using ProperTree. 

Make sure that "HS80211Family.kext" is loading first and that "AirPortAtheros40.kext" is loading after it in the config.plist. 
Note that this is case-sensitive, without it, it won’t work!

It should exactly look like this:

![Example](https://user-images.githubusercontent.com/73723350/131271107-abe28193-fd69-4ad6-ab0c-51a306b68928.png)

### Clover 
Download those 2 Kexts, "AirPortAtheros40.kext" and "HS80211Family.kext", put these into CLOVER/Kexts/Other.

## Notes
Tested with AR9287 on macOS Big Sur 11.5.1

I’m searching for people who can test those Kexts with one of the Atheros chipsets on macOS Monterey 12, if you can test it and you’ve had success with it, please DM me on Discord: sXmed#1279
