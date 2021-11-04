# qmk_dz60

## Flash the firmware
See https://qmk.fm/ for reference

- build or update your ./keymap.json file here: https://config.qmk.fm/
- copy the udev rules: `sudo cp ./50-qmk.rules /etc/udev/rules.d/`
- update the udev daemon: `sudo udevadm control --reload`
- install qmk: `python3 -m pip install --user qmk`
- run `qmk setup` and let it download the firmware repo and check your environment
- connect keyboard via USB and press the correct combination to enter bootloader
  - by default it can be space + b, both shitfs + b or others, shorting the reset pins on the back always works tho
  - in the current keymap for my dz60 it is left mod1 + left mod2 + right mod2
- run `qmk flash -kb dz60 -km [your preferred keymap name] [path to this repo]/keymap.json`
- if the command executes successfully, unplug and replug the keyboard
- test your keymap here: https://config.qmk.fm/

