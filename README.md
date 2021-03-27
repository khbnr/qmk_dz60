# qmk_dz60

## Flash the firmware
See https://qmk.fm/ for reference

- symlink or copy the [udev rules for qmk](./50-qmk.rules) to `/etc/udev/rules.d`
- install qmk: `python3 -m pip install --user qmk`
- connect keyboard via USB and press space + b to enter bootloader
- run `qmk flash -kb dz60 -km [your preferred keymap name] [path to this repo]/keymap.json`

