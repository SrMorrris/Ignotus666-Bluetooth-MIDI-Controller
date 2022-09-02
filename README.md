# Ignotus666-Bluetooth-MIDI-Controller
This is my version i have built from Ignotus666 MIDI controller:
 - Pedalboard: https://github.com/ignotus666/Bluetooth-Pedalboard
 - Desktop-controller (pots): https://github.com/ignotus666/desktop-midi-controller


 - One chip "Atmel 1284" and one HC-05 bluetooth module configured as SLAVE. For every MIDI-controller (emitter).
 - One PIC 18F-2550 and HC-05 configured as MASTER (receptor BT-USB-MIDI).One HC-05 for every MIDI-controller.
 - Multiplexer 4051.
 - Screens: - ILI 9341 2,4/2,8 inches 240x320 TFT-LCD for the pedalboard.

            - SSD1306 0,91 inches 128x32 OLED I2C (4PIN) for the desktop controller (pots).
 
The awesome controller created by ignotus666 it's my best midi controller.

This controller have one device (PIC 18F-2550) programmed as receptor bluetooth and USB-MIDI comunication. You will only have to connect the usb cable, will be recognised as BT-MIDI-receptor, no installation required.


 Every bluetooth module connected in receptor HC-05 (one per MIDI device) must be configured as MASTER.

The MIDI Controllers are chips atmel 1284 and mux 4051. One HC-05 configured as SLAVE (one per MIDI device):

 - One MIDI controller named as pedalboard_neopixel_1.13 (pedalboard): ws2812b leds, ILI9341 screen... 
 - Another Midi controller named as desktop_midi_controller (potentiometers): 128x32 I2C screen SSD1306, Analog joystick, simple leds..


## Atmel 1284

You need to build your own arduino board.

Continue..