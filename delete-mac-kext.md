# Delete MacOS Kext 


1. Enter Recovery Mode (Restart, then Command + R)

2. Open Terminal App

3. Disable System Intergrity Protection (SIP)

```
csrutil disable
```

Check to make sure it is disabled:

```
csrutil status
```


4. Restart the machine, and enter Recovery mode again

5. Delete kext in ``/Volume/MacOS/System/Library/Extentions`` folder, not ``/System/Library/Extentions``
```
rm -rf AppleIntelKBLGraphics.kext
```

6. Restart the machine, enjoy!
