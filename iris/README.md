# Layout instructions

## QMK edits

Easiest way of making changes to the keymap is to make changes using the 
[online QMK configurator](https://config.qmk.fm/#/keebio/iris/rev4/LAYOUT).

1. Go to the QMK configurator
2. Upload `kiwidamien_iris_rev4.json`
3. Make the changes
4. Download `keymap.json` from QMK configurator. Move the download back to  this folder so we can use it as a starting model next time. Note that the downloaded file will be called `kiwidamien_iris_rev4.json`
5. Now run `make copy` to compile the json keymap into a `keymap.c`, and place it in our fok of the QMK firmware app.


## Flashing instructions

To compile, run `make compile`

To flash, run `make flash`

This is for the iris (rev4) keyboard.


## Extras

We have the keymap and source files located at 
`~/qmk_firmware/keyboards/keebio/iris/keymaps/kiwidamien/`

The `rules.mk` file is located at 
`~/qmk_firmware/keyboards/keebio/iris/rev4`

`rules.mk` contains some great configurations, including the ability
to put in other source files that won't get overwritten when generating
new keymaps. See the use of SRC and the addition of `rotatary_encoder.c`

You can see the combos that we have added to the keyboard by looking at
the `combo.c` file in `kiwidamien` directory above. We can also just use
the symbolic link.
