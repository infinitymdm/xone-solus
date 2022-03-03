# xone-solus
This repository contains artifacts for building xone, an Xbox accessory driver, on Solus Linux. All credit goes to medusalix for his work [here](https://github.com/medusalix/xone). I've just packaged the thing for Solus

I've done some basic testing with my controller (model 1708) with the xbox wireless dongle. Things appear to work flawlessly, but confirmation with additional devices is desired. [Click here for the full list of supported devices](https://github.com/medusalix/xone#supported-devices).

## Installation
1. Download the most recent .eopkg from the releases page.
2. Open a terminal and `cd` to wherever you donwloaded the .eopkg.
3. Install using `sudo eopkg install xone-X.X-X-X-x86_64.eopkg`.
4. Run `sudo modprobe -r mt76x2u`. This prevents a driver conflict.
5. Run `sudo xone-get-firmware.sh`. This installs the (proprietary) firmware for the Xbox wireless dongle.
6. Profit

If you have issues installing, let me know by [creating an issue](https://github.com/infinitymdm/xone-solus/issues). All other problems (pairing, bugs, etc.) should be directed to the xone maintainers.

## Uninstalling
Simply run `sudo eopkg remove xone` to uninstall.