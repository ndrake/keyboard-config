# keyboard-config

Notes and keymap for my Kinesis Advantage w/ Stapelberg (Teensy 4.1) so I don't forget next time.

## Setup QMK build env

* Install Teensy Loader CLI: `brew install teensy_loader_cli`
* Clone QMK repo: `git clone --recurse-submodules https://github.com/qmk/qmk_firmware.git`
* Download keymap.c from this repo and place it at `keyboards/kinesis/keymaps/stapelberg/keymap.c`
* Build firmware: `util/docker_build.sh kinesis/kint41:stapelberg`
* Flash firmware: `/opt/homebrew/Cellar/teensy_loader_cli/2.2/bin/teensy_loader_cli -w -v --mcu=TEENSY41 kinesis_kint41_stapelberg.hex`
