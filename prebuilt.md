## Prebuilt Firmware
### Available Versions
These are found in [configurations.zip](https://github.com/phil-barrett/grblHAL-teensy-4.x/blob/master/configurations.zip).  

"3 axis usb quad enc" - 3 Axis, Aux Relays, Quadrature Encoder

"3 axis usb no opts" - 3 Axis, Aux Relays

"3 axis usb compat" - 3 Axis, no options, compatibility with older senders.

"4 axis usb quad enc" - 4 Axis, Aux Relays, Quadrature Encoder

"4 axis usb no opts" - 4 Axis, Aux Relays

"4 axis usb compat" - 4 Axis, no options, compatibility with older senders.

"5 axis usb quad enc" - 5 Axis, Aux Relays, Quadrature Encoder

"5 axis usb no opts" - 5 Axis, Aux Relays

"5 axis usb compat" - 5 Axis, no options, compatibility with older senders.

Ethernet versions are found in [ethernet_configurations.zip](https://github.com/phil-barrett/grblHAL-teensy-4.x/blob/master/ethernet_configurations.zip).

"3 axis eth quad end" - 3 Axis, Ethernet, Quadrature Encoder

"3 axis gangY eth quad enc" - 3 Axis, Axis B ganged to Y, Ethernet, Quadrature Encoder

"4 axis eth quad enc" - 4 Axis, Ethernet, Quadrature Encoder

"4 axis gangY eth quad enc" -4 Axis, Axis B ganged to Y, Ethernet, Quadrature Encoder

"5 axis eth quad enc" - 5 Axis, Ethernet, Quadrature Encoder

### Options
n Axis - number of axes

usb - USB interface

quad enc - Quadrature encoder on digital inputs. Supports spindle and feed rate override.

no opts - basic support

Compat - Sender compatibility.  disables new features of grblHAL and maintains compatibility with senders.

eth - Ethernet support

More options will be added in the future.

### Loading Firmware onto a Teensy 4.1
Follow these basic steps:
1. Download the [firmware configurations file](https://github.com/phil-barrett/grblHAL-teensy-4.x/blob/master/configurations.zip) and extract the contents.
2. Select the .hex file that coresponds to the features you will use.
3. Obtain the Teensy Loader for your platform.
4. Use the loader to load the .hex file into your Teensy.

See the platform sections for details and hints.

#### Windows 
Download Teensy.exe from the [PJRC Website here](https://www.pjrc.com/teensy/loader_win10.html). The page may say Windows Vista but it works for all recent Windows versions.
Plug in your Teensy 4.1 via USB. Find Teensy.exe and run it.  It should open as a small window. In File/Open HEX File, select and open the .hex file you want and press OK. Then, press the button on the Teensy 4.1. You are ready to test it now. 

#### Macintosh OS X
Macintosh instructions [are here](https://www.pjrc.com/teensy/loader_mac.html). Plug in your Teensy 4.1 via USB. Follow the instructions to install and run the loader. It should open as a small window. Then, from the File name, choose "Open HEX File" and open the .hex file you want and press OK. Select "Program" from the "Operations" menu, or click the Program button on the tool bar. It should display a brief loading message. You are ready to test it now

#### Linux
Instructions for Ubuntu [are here](https://www.pjrc.com/teensy/loader_linux.html). Other Linux versions work though you will need to build the loader for your platform.  The [instructions and links to the github repository are here.](https://www.pjrc.com/teensy/loader_cli.html)
