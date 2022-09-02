# Ignotus666-Bluetooth-MIDI-Controller
This is my version i have built from Ignotus666 MIDI controller.

 - Atmel 1284 and HC-05 bluetooth module configured as SLAVE. 
 - PIC 18F-2550 and HC-05 configured as MASTER.
 - 2 Multiplexer 4051
 
The awesome controller created by ignotus666 it's my best midi controller.

This controller have one device (PIC 18F-2550) programmed as receptor bluetooth (serial) and USB-MIDI comunication. You will only have to connect the usb cable, recognised as BT-MIDI-receptor, no installation required. Every bluetooth module connected in receptor HC-05 (one per MIDI device) must be configured as MASTER.

Another devices are atmel 1284 and mux 4051. One HC-05 configured as SLAVE (one per MIDI device):

 - One device named as pedalboard_neopixel_1.13 (pedalboard): ws2812b leds, ILI9341 screen. 
 - Another device named as desktop_midi_controller (potentiometers): 128x32 I2C screen SSD1306, Analog joystick.
