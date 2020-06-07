# arduino-konami-spoof
 Drop in library to replicate IIDX and SDVX controllers using Arduino.
 
 This library only works with the Leonardo and Micro (or Leo / Micro / Pro Micro clones).
 
 This includes core files from Arduino Core 1.8.2.

## HOW TO INSTALL

 Close the Arduino IDE and place the `arduino-konami` folder into your local hardware folder.  
 On a typical Arduino install, this is located in `Documents\Arduino\hardware`.  
 On portable installations, this is located in `arduino\portable\sketchbook\hardware`.

 Restart the Arduino IDE and select the appropriate board from `Tools -> Board -> Konami Controllers`.
 
 Then, simply use any standard joystick library to play the game as normal. [MHeironmius's Library](https://github.com/MHeironimus/ArduinoJoystickLibrary) works well.
 
## HOW TO USE

### IIDX

 The following must be adhered to:
| Joystick Button | SDVX Key |
|:---------------:|:--------:|
| B1              | KEY 1    |
| B2              | KEY 2    |
| B3              | KEY 3    |
| B4              | KEY 4    |
| B5              | KEY 5    |
| B6              | KEY 6    |
| B7              | KEY 7    |
| B9              | KEY E1   |
| B10             | KEY E2   |
| B11             | KEY E3   |
| B12             | KEY E4   |
| X-AXIS          | TT       |

### SDVX

 The following must be adhered to:
| Joystick Button | SDVX Key |
|:---------------:|:--------:|
| B1              | BT A     |
| B2              | BT B     |
| B3              | BT C     |
| B4              | BT D     |
| B5              | FX L     |
| B6              | FX R     |
| B9              | START    |
| X-AXIS          | VOL-L    |
| Y-AXIS          | VOL-R    |

## HOW TO REVERT

 When you wish to revert the board back to a normal state, begin an upload for a normal Arduino sketch and restart the board by shorting the RST pin to GND, or by pressing the Reset button if your board has one.
 
## Credits

 [Arduino Core](https://github.com/arduino/ArduinoCore-avr)  
 [Ziemas](https://github.com/Ziemas) for the IIDX profile  
 [SirusDoma](https://github.com/SirusDoma) for the SDVX profile
