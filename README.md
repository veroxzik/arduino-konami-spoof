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

 At this time I am unsure of the controller mapping-- a PR with the correct keys would be appreciated!
 
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


## HOW TO REVERT

 When you wish to revert the board back to a normal state, begin an upload for a normal Arduino sketch and restart the board by shorting the RST pin to GND, or by pressing the Reset button if your board has one.
 
## Credits

 [Arduino Core](https://github.com/arduino/ArduinoCore-avr)  
 [Ziemas](https://github.com/Ziemas) for the IIDX profile  
 [SirusDoma](https://github.com/SirusDoma) for the SDVX profile