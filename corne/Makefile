KEYBOARD_NO_REV=crkbd
KEYBOARD=$(KEYBOARD_NO_REV)/rev1
JSON=kiwidamien_corne.json
DEST=$(HOME)/qmk_firmware/keyboards/$(KEYBOARD_NO_REV)/keymaps/kiwidamien/keymap.c


copy: $(JSON)
	qmk json2c $(JSON) -o $(DEST)

compile:
	qmk compile -kb $(KEYBOARD)

flash:
	qmk flash -kb $(KEYBOARD)
	
