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
   


- Quartz crystal  16 mhz (you can choose another type, see this page: https://github.com/MCUdude/MightyCore ):

   ![crystal16mhz](https://user-images.githubusercontent.com/80991642/188249683-4184b998-f497-49fb-9cb6-9cccf182c4fd.png)



- 2 capacitors. 22 picofarads:

   ![22pf](https://user-images.githubusercontent.com/80991642/188249695-0400bfaf-fe53-4ffe-8346-dbfa276bd8d5.png)



- 1 capacitor. 10 microfarads:

   ![capacitor10microfarads](https://user-images.githubusercontent.com/80991642/188249796-e83dd31e-6677-4dcb-bcf7-218a2875536a.png)



- 1 resistor. 10 kiloohmios  (1/4  watt it's good):

    ![resistor10k](https://user-images.githubusercontent.com/80991642/188249926-cb25b5dc-9841-40eb-8c46-fd5cb1ba9a70.png)



- 1 FTDI-USB or 1 Arduino UNO (burn bootloader/upload sketches).
 - FTDI-USB:

   ![50281](https://user-images.githubusercontent.com/80991642/188249442-33d0131b-d722-4c33-a3ae-b85d3bdb62e0.jpg)


 - Arduino uno:

   ![50272](https://user-images.githubusercontent.com/80991642/188249457-9497a595-dc3b-4a73-a059-714f899d7a8d.png)


- Board, wire, conectors, solder wire, etc..

Build your board it's so easy..You can follow this map:

![atmel1284](https://user-images.githubusercontent.com/80991642/188251934-33c12f08-5b4e-4bc5-853b-1596b3b50b9a.png)

For other atmel chips 328/644 etc.. it's mostly the same components, but different PINOUT:

![standalone_arduino](https://user-images.githubusercontent.com/80991642/188252001-dbb5c8e9-f86c-4651-bfc5-4fd15e57db5c.png)


Then, you need to install this board in your pc, so you can choose it for compile.

There's so much types (sanguino,bob,etc..) now i will show you which one worked for me like a charm.

You need to visit this page and follow instructions, (For install 1284 board):

https://github.com/JChristensen/mighty-1284p/tree/v1.6.3

Then you can choose this type of board in your Arduino IDE:

![50264](https://user-images.githubusercontent.com/80991642/188249777-cf47c496-3979-4035-b6fd-4994014b81d4.png)

Choosing a COM port and then your type of programmer you are now able to upload sketeches or burn the bootloader for the first time..


## Choosing a FTDI-USB for burn bootloader/ upload sketches (1284P).

A Ftdi-usb programmer it's a very good and cheap solution for upload sketches..(or burn the bootloader).

You will need to burn the bootloader the first time you connect the chip, and then you can upload sketches everytime you want.

Here you can see how to connect an ftdi-usb (the 1284p it's mostly the same schematic, you can follow this picture):

![50279](https://user-images.githubusercontent.com/80991642/188249448-69ef2be5-8227-47bc-89f0-d9d214c05c21.png)

If you have problems with pin-numbered. i bring you this other picture:

![ftdi-usb chip atmel](https://user-images.githubusercontent.com/80991642/188252661-82feb4ad-9cb0-47b4-8fa5-3b5c7b71b41f.png)

You connect the ftdi-usb to the pc and open Arduino IDE:
-Select your board (maniacbugh mighty 1284 etc..).
-Select your COM port (mine COM 10)
-Select your type of programmer (ftdi-usb):AVRISPMKII

![50280](https://user-images.githubusercontent.com/80991642/188249528-60330d37-2c5e-4091-b843-7455989ad99a.png)

And you can select "burn bootloader" and then you can upload sketches , for example you can upload an ARDUINO-IDE Basics-example for test your board:
Open examples "blink" and connect one led to see what happen...

## Choosing an Arduino UNO for burn bootloader/ upload sketches (1284P).

If you got an arduino uno it's the best solution i think..
If you want to upload an sketch with arduino UNO, you must press SHIFT and then the upload button (Arduino IDE)

This picture it's for connect an arduino UNO:

![50278](https://user-images.githubusercontent.com/80991642/188249563-389d8151-8595-4c84-b004-f8b0d7cfb937.gif)

    NOTE: Don't forget the 10 microfarads electrolytic capacitor (there it's not in this picture..)


You connect the arduino uno to the pc and open Arduino IDE:
-Select your board (maniacbugh mighty 1284 etc..).
-Select your arduino uno COM port (mine COM 4)
-Select your type of programmer (arduino uno):arduinoasisp

![50265](https://user-images.githubusercontent.com/80991642/188249494-11ef6aab-b6cb-476d-9aaa-a431de221bf3.png)

And you can select "burn bootloader" and then you can upload sketches , for example you can upload an ARDUINO-IDE Basics-example for test your board:
Open examples "blink" and connect one led to see what happen...

![50274](https://user-images.githubusercontent.com/80991642/188249413-04938af2-d0fe-452e-9daa-710ddca12211.jpg)


# Your battery circuit

 to be continuoso, pues no mas