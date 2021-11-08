# Flashing instructions

You will usually want to make layout changes in [QMK configurator](https://config.qmk.fm/#/ai03/equinox/rev0/LAYOUT_all) online,
instead of trying to manually edit the keymap by hand. 

1. Go to the QMK configurator page
2. Upload `keymap.json` from this repo
3. Make the changes
4. Download `keymap.json` from QMK configurator. Move the download back to this folder so that we can use it as a starting point
5. Now use `qmk` to get a `keymap.c` file:
   ```bash
   qmk json2c keymap.json -o ~/qmk_firmware/keyboards/keebio/iris/keymaps/kiwidamien/keymap.c
   ```

This will get us ready for the compile and flash!

## Compiling

You can run this command anywhere on your system:
```bash
qmk compile
```

## Flashing

You will need to do this twice, once with each side of the keyboard

1. Press the button on the underside of the keyboard that is plugged in to power
2. Run `qmk flash`

Unplug the half of the keyboard you were using, and plug in the other side. Repeat instructions.

You have now flashed your iris keyboard!
