![logo](https://user-images.githubusercontent.com/80991642/188264119-e3f64080-294c-4dc2-a61c-32a80d3abbd1.png)


# Ignotus666-Bluetooth-USB-MIDI-Controller. The SUPER-COBRA, 

This it's the second device i have built. It's my best Midi-controller.

Ignotus666 is his creator:   https://github.com/ignotus666

The philosophy of this controller it's simple:


- One device named as receptor will be the Bluetooth-USB midi signal receptor, this device receives the serial signal from the midi controllers (tx and rx pins), through the hc-05 (master) and transforms this signal into midi and send it into the pc via Usb cable.


- The other devices are one chip atmel 1284 (one per midi-controller) and one hc-05 configured as SLAVE (one per midi-controller). You can build so many controllers as you want...(one master = one slave)


## The pedalboard

First, you must download the code from ignotus666 github:

https://github.com/ignotus666/Bluetooth-Pedalboard

You can watch how to build your pedalboard on his github repository, and here i bring you how i have built mine
(my experience)

![20220812_021333](https://user-images.githubusercontent.com/80991642/188260381-aee3cd93-18c4-4671-8aab-070a11c7b0e7.jpg)

![Sin nombre34](https://user-images.githubusercontent.com/80991642/188267227-4c6f0bac-434f-4efe-aeae-00c80574a7e2.png)

![Sin nombreñl](https://user-images.githubusercontent.com/80991642/188267291-d2734cc1-4102-4c43-b103-8e386fd9a87f.png)


You can download every file in the .zip , but you can see the components list here:

https://drive.google.com/uc?id=1DSQUBxHxhUGM9xNX7fbMygEOfUKrwz3I&export=download

This Midi controller (pedalboard)has got one atmel 1284 and one hc-05 configured as SLAVE, one mux 4051 and one
screen ILI 9341 2,4/2,8 inches 240x320 TFT-LCD .

You can see schematics here:

https://photos.google.com/search/_tra_/photo/AF1QipMGrOhExx-JlsJZWpQXzOmH4l8pAK77iXgN28EQ


In the .zip there's some gimp files and .png files, located in ARTWORK (if you want to use some pictures for your controller).

Working images with gimp in layers, it's so easy..

- Install gimp:

https://www.gimp.org/


![20220812_014343](https://user-images.githubusercontent.com/80991642/188267579-655b3772-8dfb-4f6f-a327-1094c434e66e.jpg)

![20220812_014419](https://user-images.githubusercontent.com/80991642/188267587-6c0ea1ec-15d8-4772-b7d3-516c819ab902.jpg)

![20220812_014301](https://user-images.githubusercontent.com/80991642/188267564-a064bae2-b2f3-4165-ad23-21d94b5ca6d6.jpg)


## The Desktop Controller (pots)

![Sin nombrefrr](https://user-images.githubusercontent.com/80991642/188267988-86a20ed8-bd0d-41e7-a6f9-08789fad2e46.png)

First, you must download the code from ignotus666 github:

- Desktop-controller (pots): https://github.com/ignotus666/desktop-midi-controller

You can watch how to build your pedalboard on his github repository, and here i bring you how i have built mine

![Sin nombrefdfdfd](https://user-images.githubusercontent.com/80991642/188267737-b5842383-3834-4798-9bec-64b2ed29dc98.png)

![Sin nombre66](https://user-images.githubusercontent.com/80991642/188261036-c0f9c550-f15b-4ef5-881b-310eff8469e9.png)

![Sin nombredr](https://user-images.githubusercontent.com/80991642/188267695-44a8b14c-68b7-4afe-93f6-9410b43c6ff4.png)


You can download the components list here:

https://drive.google.com/uc?id=1LK4GFyihy7jwFu3tx3JY8D9s9N_1IbXA&export=download

This Midi controller (desktop controller) one atmel 1284 and one hc-05 configured as SLAVE, one mux 4051 and 
screen SSD1306 0,91 inches 128x32 OLED I2C (4PIN).

You can see schematics here:

https://photos.google.com/search/_tra_/photo/AF1QipPfj81Rz_Q_teM37dQCxnwQC3Gwz5QAASjpksV0

You can find some gimp and .png files in ARTWORK

![Sin títulogfg](https://user-images.githubusercontent.com/80991642/188267779-b280c873-fd3a-4933-aac7-c5f3f1bca042.png)

![Sin nombredfsgdfga](https://user-images.githubusercontent.com/80991642/188267820-eaf329f7-c51c-418f-8586-63ee0299132f.png)

![Sin nombrefasdfas](https://user-images.githubusercontent.com/80991642/188267898-e016f619-ab78-455c-b0d3-3cdac76cbaf9.png)



## The receptor Bluetooth USB Midi.

The instructions about how to build the receptor are in the ignotus666 repository, you will find it on both files (pedalboard and desktop-controller):

https://github.com/ignotus666/desktop-midi-controller

https://github.com/ignotus666/Bluetooth-Pedalboard

You can download the components list here:

https://drive.google.com/uc?id=17Sct6pLxF_GxMCLaB8IY5S19NntpqlOr&export=download

The receptor Bluetooth USB-MIDI,has got one PIC 18F-2550 and modules hc-05 configured as MASTERS, don´t forget to connect one led to STATE pin and GND (for check bluetooth link).

The receptor have one chip (PIC 18F-2550) programmed as receptor bluetooth and USB-MIDI comunication. 

You will only have to connect the usb cable, and will be recognised as BT-MIDI-receptor, no installation required.


 Every bluetooth module HC-05, connected in receptor (one per MIDI device) must be configured as MASTER.


You can see schematics here:

https://photos.google.com/search/_tra_/photo/AF1QipPQdP5PnPhRYeayPkFFX1c2DS-Jxpb-6Q2AOWZB



So let's resume..



 - One chip "Atmel 1284" and one HC-05 bluetooth module configured as SLAVE. For every MIDI-controller (emitter). 


 - One PIC 18F-2550 and modules HC-05 configured as MASTER (receptor BT-USB-MIDI).One HC-05 MASTER for every MIDI controller (slave).
      
 
This awesome controller created by ignotus666 it's my best midi controller.



The MIDI Controllers are chips atmel 1284 and also mux 4051, and  one HC-05 configured as SLAVE (one per MIDI device):

 - One MIDI controller will be named as pedalboard_neopixel_1.13 (pedalboard): ws2812b leds, ILI9341 screen,atmel1284, mux4051, etc...


 - Another Midi controller named as desktop_midi_controller (potentiometers): 128x32 I2C screen SSD1306, Analog joystick, leds, atmel1284, mux4051, etc..

 - You can build more midi controllers, if you want. you only need to put one hc-05 configured as master in the receptor and build your midi device and put one hc-05 configured as slave.


## Building the Atmel 1284p board

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

![55780551-868e7780-5aa8-11e9-88bf-19ad038e9f07](https://user-images.githubusercontent.com/80991642/188256813-0a3e9ac0-c131-4daa-b03a-8c45820d8b39.png)


Then, you need to install this board in your pc, so you can choose it in arduino IDE. 

There's so much types 1284(sanguino,bob,etc..) now i will show you which one worked for me like a charm.

You need to visit this page and follow the instructions, (for install 1284 board):

https://github.com/JChristensen/mighty-1284p/tree/v1.6.3

Then you can choose this type of board in your Arduino IDE:

![50264](https://user-images.githubusercontent.com/80991642/188249777-cf47c496-3979-4035-b6fd-4994014b81d4.png)

Then you choose your COM port and then your type of programmer you are now able to upload sketeches or burn the bootloader for the first time..

![6c4cedc24facf84159bee620e88f1-2807213](https://user-images.githubusercontent.com/80991642/188256789-306f5176-0955-4335-be45-ed9dae5521f0.png)


## Choosing a FTDI-USB for burn bootloader/ upload sketches (1284P).

A Ftdi-usb programmer it's a very good and cheap solution for upload sketches..(or burn the bootloader for the first time).

You will need to burn the bootloader the first time you connect the chip, and then you can upload sketches everytime you want.

Here you can see how to connect an ftdi-usb (the 1284p it's mostly the same schematic, you can follow this picture):

![50279](https://user-images.githubusercontent.com/80991642/188249448-69ef2be5-8227-47bc-89f0-d9d214c05c21.png)

If you have problems with pin-numbered. i bring you this other picture:

![ftdi-usb chip atmel](https://user-images.githubusercontent.com/80991642/188252661-82feb4ad-9cb0-47b4-8fa5-3b5c7b71b41f.png)

You connect the ftdi-usb to the pc and open Arduino IDE:


- Select this board ("maniacbug" Mighty 1284p 16MHz using Optiboot):

- Select your COM port (mine it's COM 10):

- Select your type of programmer (ftdi-usb):AVRISPMKII:

![50280](https://user-images.githubusercontent.com/80991642/188249528-60330d37-2c5e-4091-b843-7455989ad99a.png)


And you can select "burn bootloader" and then you can upload sketches.

For example.. you can upload the Arduino IDE Basics-example, "Blink", for test your board:

![6374404c5374b3991cbb44f9265f0-2807213](https://user-images.githubusercontent.com/80991642/188256783-b4ee56a9-1bf6-4a29-9ea8-c12059b917c1.png)

Open and upload the example "blink", and connect one led to pin 13 and GND to see what happen...

## Choosing an Arduino UNO for burn bootloader/ upload sketches (1284P).

If you got an arduino uno.. it's the best solution i think..

### First you must prepare your arduino board

 - Open arduino IDE and select the COM port where it's connected the arduino uno. (my case COM 4).

 - Select the BOARD type (TOOLS---BOARD---ARDUINO UNO):Select Arduino UNO.

 - Select FILE---EXAMPLES and choose "ARDUINO ISP"

 - Upload the sketch into the arduino UNO.

 - Finished. you have got a arduino uno programmer for the atmel 1284p (burn bootloader/upload sketches)


If you want to upload an sketch into the 1284p with arduino UNO as programmer, you must press SHIFT and then the upload button (in Arduino IDE).

![f387d02e1e32b2d08365066c6ffb0-2807213](https://user-images.githubusercontent.com/80991642/188256776-f04fb77f-a90d-4dd8-8e4f-3c0297392187.png)

This picture it's for connect an arduino UNO to the 1284p and program the 1284p:

![50278](https://user-images.githubusercontent.com/80991642/188249563-389d8151-8595-4c84-b004-f8b0d7cfb937.gif)

    NOTE: Don't forget the 10 microfarads electrolytic capacitor (there it's not in this picture..) and the resistor 10K for the pin reset (also not in the picture)


Then you connect the arduino uno to the pc and open Arduino IDE:


- Select your board ("maniacbug" Mighty 1284p 16MHz using Optiboot).

- Select your arduino uno COM port (mine it's COM 4).

![627617618ef5594a886fa27a3e469-2807213](https://user-images.githubusercontent.com/80991642/188256798-4e7f54f2-b962-4b8d-b514-0a0748d776e0.png)

- Select your type of programmer (arduino uno):"ARDUINO AS ISP".

![50265](https://user-images.githubusercontent.com/80991642/188249494-11ef6aab-b6cb-476d-9aaa-a431de221bf3.png)

And you can select "burn bootloader" and then you can upload sketches.


For example you can upload an ARDUINO-IDE Basics-example for test your board:


Open examples "blink" and connect one led to see what happen...

![50274](https://user-images.githubusercontent.com/80991642/188249413-04938af2-d0fe-452e-9daa-710ddca12211.jpg)


# Your battery circuit

 You can choose whatever battery you want (3/5 volts i's good).

  - 18650 batteries.

   ![18650](https://user-images.githubusercontent.com/80991642/188254935-aa8c37af-5d47-4382-b714-c8a6a0ac6fdf.png)

  - Old batteries (mobile, tablet, etc..). But please...Be careful..

   ![50329](https://user-images.githubusercontent.com/80991642/188254926-39bac28b-aa3a-4872-b346-302078142226.jpg)

   You will need a usb module charger, TP-4056, it's good and cheap.

   ![4056module](https://user-images.githubusercontent.com/80991642/188254992-ab0ab3f9-a17c-4975-9eee-0e788d9f2140.png)

   You connect a usb cable and you can charge your batteries (red light-charging/blue light-charge complete).


   You also need a booster, MT-3608.

   ![50413](https://user-images.githubusercontent.com/80991642/188255087-ef10ed31-d8c9-4d24-85c6-f3923262dbae.jpg)

    This booster must be regulated..read the voltage at the output and turn the screw until voltage downs to +5v.
    Be careful... because this boosters gives +20 volts if you dont turn the screw, (+20 volts it´s to kill the chip). Be sure to read +5v or less at the output.

   And here you can see the full circuit:

   ![CIRCUITOBATERIA](https://user-images.githubusercontent.com/80991642/188255284-29e71dac-d7cc-421a-81ea-227b5371676d.png)


   # Configure HC-05 bluetooth module

  Be aware that certain kind of HC-05 modules can´t be configured as MASTER. Are only Slaves.

  The newest versions HC-05 and the HC-06 can´t be configured as MASTER.


  We will need 2 HC-05 modules for every single MIDI controller we make..

   - One hc-05 will be configure as MASTER and will be on the BT-USB-MIDI receptor (the PIC 18F-2550).

   - The other one module will be configure as SLAVE and will be in the Midi Controller device.

You can configure your HC-05 modules with a FTDI-USB programmer or an arduino uno, as well.

If you use a ftdi-usb you must switch the ftdi device into 3,3v (change jumper mode). the conexion it´s so easy.. (arduino uno and ftdi):

![d1d1fb109c9ba1eba90b1db717026-2815846](https://user-images.githubusercontent.com/80991642/188258766-ac7b043d-4a80-4a60-b948-4f40b3ee130f.jpg)

- RX(FTDI)-----RX(HC-05).

- TX(FTDI)-----TX(HC-05).

- +5V(FTDI)----+5V(HC-05).

- GND(FTDI)----GND(HC-05).

    - NOTE: Don't forget to put the ftdi jumper into 3,3 volts mode.


Ok..you must know there's so much types of HC-05 modules..

But every model, i think.., you must press one button on the module-board before turning on the module and then release the button. In order to enter the device into "AT MODE"

When hc-05 it´s in at-mode you can see the red led on the module, flashing slowly.

Open your arduino ide and open serial monitor (com-port must be correct selected, no problem with the programmer type or the board-type, you can select whatever type, no problem).

Then you have to select "BOTH NL AND CR".
And select the correct bauds speed (for me i see words correctly at 38400bds)(maybe you see words correctly on 9600bds).

Then. You must type:

AT

And if you see an answer (OK) everything it's fine.. can move forward...

### Let's start to configure the HC-05 bluetooth module

A important component of this controller it's the HC-05 module, and must be configured.

- In the serial monitor (arduino ide), type this:

    AT+NAME=PepeHeredia

Your device will be name as PepeHeredia

- Then, type this:

AT+ROLE=1

And after type this:

AT+ROLE?

If you see AT+ROLE=1 your hc-05 module can be configured as MASTER (AT+ROLE=1 MASTER/ AT+ROLE=0 SLAVE)

- This time let's configure the bauds speed comunication, type this:

AT+UART=115200,0,0

- If you type this:

AT+PSWD=4567

You will change the pin pswd connexion to 4567

- More...now type this:

AT+ADDR?

And you will see the MAC hc-05 module address. Write it in a paper you will need it when configure the SLAVE module. But you must know you have to change every word in the MAC address, every word must be on capital words..

For example my master hc-05 module it´s: 98da:78:013ba 

but really it's:  98DA:78:013BA    (all words are always capital words, remember..)

- Now let's configure AT+CMODE (1=conexion everywhere/ 0= only bind conexions ).

- And if you choose bind conexions (i think it's the best)..

AT+BIND=98DA:50:0126BA       (98DA:50:0126BA it´s the hc-05 SLAVE module MAC addres).


If you finished your configuration type AT+RESET..

You can test your bluetooth link with a led (connected to STATE and GND). When bluetooth module it's linked.. the led will be on.


