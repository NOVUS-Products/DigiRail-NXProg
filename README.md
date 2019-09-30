# DigiRail NXprog

## This repository
This repository presents some useful information about NOVUS DigiRail NXprog, like user guide, examples and the *Board Manager* file to download.

The user guide is a short version in English, which only shows the functions that can be used and a resume of how to use DigiRail NXprog.


## Installation

### Driver Installation

#### Windows

1. Download the [signed drivers](https://github.com/NOVUS-Products/DigiRail-NXprog/drivers) and unzip into any folder.
   Note that the Windows 10 generic CDC drivers work as well.
1. Plug in the NXprog.
1. Windows will detect the board. 

#### Linux

1. No driver installation is needed.


### NOVUS NXprog Core installation


1. The NOVUS NXprog Core requires Arduino IDE 1.6.7 or above (including 1.8.x).
1. Download [Arduino Desktop IDE](https://www.arduino.cc/en/Main/Software)
3. Follow the download and installation guidelines as described in [Install the Arduino Desktop IDE](<https://www.arduino.cc/en/Guide/HomePage>) 
4. After installation in the Arduino IDE, click File->Preferences.
5. Click the button next to Additional Boards Manager URLs.
6. Add the reference to NOVUS platform definition https://raw.githubusercontent.com/NOVUS-Products/DigiRail-NXprog/master/platforms/NXprog.json
7. Save preferences, then open the Boards Manager.
8. Install the NOVUS Arduino package.
9. Close Boards Manager, then click Tools->Board->(choose board).
10. Select the MCU with the now visible Tools->Microcontroller menu (if present).
11. Plug in the NXprog.
12. Click Tools->Port and choose the COM port. Note that the board indicated may not match the chosen board*
13. You can now upload your own sketch.


## Language reference
The NXprog version Arduino programming language is an extension of standard [Arduino Language](https://www.arduino.cc/reference/en/) can be divided in three main parts: 
* IO Functions
	* [Standard Analog](./AnalogIO.md)
	* [Expert IO](./ExpertAnalogIO.md)
* Values 
	* [Sensor Type](./SensorType.md)
* Structures
	* [Analog Configuration](./AnalogConfiguration.md)
