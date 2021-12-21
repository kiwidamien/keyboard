KEYBOARD_NO_REV=keebio/iris
KEYBOARD=$(KEYBOARD_NO_REV)/rev4
JSON=kiwidamien_iris_rev4.json
DEST=$(HOME)/qmk_firmware/keyboards/$(KEYBOARD_NO_REV)/keymaps/kiwidamien/keymap.c


copy: $(JSON)
	qmk json2c $(JSON) -o $(DEST)

compile:
	qmk compile -kb $(KEYBOARD)

flash:
	qmk flash -kb $(KEYBOARD)
	
