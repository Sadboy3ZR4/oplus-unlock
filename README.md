# Enable fastboot on oplus devices
Script to disable fastboot unlock verification of oplus LK images ([web version](https://lkpatcher.r0rt1z2.com/)).

## Installation
```bash
sudo apt install python3-pip
pip3 install --upgrade git+https://github.com/R0rt1z2/oplus-unlock
```

## Usage
```bash
oplus-unlock lk.bin [-o patched_lk.bin] [-p patches.json]
```
> *(arguments between brackets are optional, use `h` to view full usage).*

## Notes
* This tool requires unlocked seccfg to work (i.e: your device must have been previously unlocked with mtkclient).
* To flash the modified image, use [mtkclient](https://github.com/bkerler/mtkclient). Note that flashing modified LK images with locked seccfg will result in a brick.
* Use this tool at your own risk. I am not responsible for bricked devices. Please **BACKUP** your bootloader before using this tool.
* `patches.json` contains example patches, you can modify it and add your own.

## License
* This tool is licensed under the GNU (v3) General Public License. See `LICENSE` for more details.