# Ignotus666-Bluetooth-USB-MIDI-Controller
This is my second device, i have built from Ignotus666 MIDI controller:

I will show you how i have built mine, but you must first download the code from ignotus666 repository:

 - Pedalboard: https://github.com/ignotus666/Bluetooth-Pedalboard

 - Desktop-controller (pots): https://github.com/ignotus666/desktop-midi-controller


 - One chip "Atmel 1284" and one HC-05 bluetooth module configured as SLAVE. For every MIDI-controller (emitter).
 - One PIC 18F-2550 and HC-05 configured as MASTER (receptor BT-USB-MIDI).One HC-05 for every MIDI-controller.
 - Multiplexers 4051.
 - Screens: - ILI 9341 2,4/2,8 inches 240x320 TFT-LCD for the pedalboard.

            - SSD1306 0,91 inches 128x32 OLED I2C (4PIN) for the desktop controller (pots).
 
This awesome controller created by ignotus666 it's my best midi controller.

This controller have one device (PIC 18F-2550) programmed as receptor bluetooth and USB-MIDI comunication. 

You will only have to connect the usb cable, and will be recognised as BT-MIDI-receptor, no installation required.


 Every bluetooth module HC-05, connected in receptor (one per MIDI device) must be configured as MASTER.

The MIDI Controllers are chips atmel 1284 and mux 4051. One HC-05 configured as SLAVE (one per MIDI device):

 - One MIDI controller named as pedalboard_neopixel_1.13 (pedalboard): ws2812b leds, ILI9341 screen... 
 - Another Midi controller named as desktop_midi_controller (potentiometers): 128x32 I2C screen SSD1306, Analog joystick, leds..


## Atmel 1284

You need to build your own arduino board. Components list:

- Chip atmel 1284p (here you can see the atmel1284 chip and the whole board soldered with all components):
   ![50269](https://user-images.githubusercontent.com/80991642/188249419-77d77173-d762-4c7a-ac24-bf12f1ca94e5.jpg)
   ![50270](https://user-images.githubusercontent.com/80991642/188249431-49a746da-f2ef-42df-be08-a2381003fa6e.png)
- Quartz crystal  16 mhz (you can choose another type, see this page: https://github.com/MCUdude/MightyCore ):
   ![crystal16mhz](https://user-images.githubusercontent.com/80991642/188249683-4184b998-f497-49fb-9cb6-9cccf182c4fd.png)
- 2 capacitors. 22 picofarads:
   ![22pf](https://user-images.githubusercontent.com/80991642/188249695-0400bfaf-fe53-4ffe-8346-dbfa276bd8d5.png)
- 1 capacitor. 10 microfarads:
   ![capacitor10microfarads](https://user-images.githubusercontent.com/80991642/188249796-e83dd31e-6677-4dcb-bcf7-218a2875536a.png)
- 1 resistor. 10 kiloohmios  (1/4  watio it's good).
   ![resistor10k](https://user-images.githubusercontent.com/80991642/188249926-cb25b5dc-9841-40eb-8c46-fd5cb1ba9a70.png)
- 1 FTDI-USB or 1 Arduino UNO (burn bootloader/upload sketches).
 - FTDI-USB:
   ![50281](https://user-images.githubusercontent.com/80991642/188249442-33d0131b-d722-4c33-a3ae-b85d3bdb62e0.jpg)


 - Arduino uno:
   ![50272](https://user-images.githubusercontent.com/80991642/188249457-9497a595-dc3b-4a73-a059-714f899d7a8d.png)


- Board, wire, conectors, solder wire, etc..
