# xone-solus
This repository contains artifacts for building xone, an Xbox accessory driver, on Solus Linux. All credit goes to medusalix for his work [here](https://github.com/medusalix/xone). I've just packaged the thing for Solus.

I've done some basic testing with my controller (model 1708) with the xbox wireless dongle. Things appear to work flawlessly, but confirmation with additional devices is desired. [Click here for the full list of supported devices](https://github.com/medusalix/xone#supported-devices).

## Installation

xone is available from the official Solus repository. Since it's a kernel module, you'll need to figure out which version of the Linux kernel you're using.

Solus provides two kernel packages: LTS and Current. If you don't know which one your system is using, open a terminal and run `uname -r`. If the output ends in `current`, you'll want the `xone-current` package. If it ends in `lts`, you'll want the `xone` package. Both can be found in Software Center, or by using `eopkg`.
