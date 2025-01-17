NEOS
======

NEOS is the operating system for your [comma two](https://comma.ai/shop/products/comma-two-devkit) and [EON Gold Dashcam Development Kit](https://comma.ai/shop/products/eon-gold-dashcam-devkit).

Updates
------

When openpilot requires a NEOS update, you won't have to do anything. NEOS updates download in the background auotmatically, just like normal openpilot updates. This repo is for restoring or recovering your device.

Restoring on macOS & Linux
------

1. Connect your comma two (via a USB-C to USB-A cable) or EON Gold (via a USB-mini-B to USB-A cable) to your computer
2. Open a terminal
3. Clone this repo `git clone https://github.com/commaai/eon-neos.git`, then `cd eon-neos`
4. Run `./download.py`
5. Put your device into fastboot mode by turning off your device, then holding volume down + power.
6. Run `./flash.sh` DO NOT DISCONNECT THE DEVICE!

Restoring on Windows
------
1. Install the Google USB driver for ADB (Android Debug Bridge)... https://developer.android.com/studio/run/win-usb
2. Connect your comma two (via a USB-C to USB-A cable) or EON Gold (via a USB-mini-B to USB-A cable) to your computer
3. Download and extract this repository
4. Download & install Python 3
5. Run download.py to download NEOS and flashing tools
6. Put your device into fastboot mode by turning off your device, then holding volume down + power.
7. Run flash.ps1 (right click, run with powershell). DO NOT DISCONNECT THE DEVICE!

```
git clone git clone git@github.com:kuasha/eon-neos.git
git checkout r081

$./download.py 
downloading https://commadist.azureedge.net/neosupdate/recovery-db31ffe79dfd60be966fba6d1525a5081a920062b883644dc8f5734bcc6806bb.img with hash db31ffe79dfd60be966fba6d1525a5081a920062b883644dc8f5734bcc6806bb
..hash check pass
downloading https://commadist.azureedge.net/neosupdate/ota-signed-e28337bbf4c776940f10562437b53cc61e7ae25752fc96897bd350296fa41292.zip with hash e28337bbf4c776940f10562437b53cc61e7ae25752fc96897bd350296fa41292

$./flash.sh
[8:53 PM]
https://smiskol.com/fork/commaai/v0.8.1
```
