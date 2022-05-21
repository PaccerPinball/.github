# Paccer

This organisation hosts various repositories for our "Paccer" Pinball, a DIY (wood) project. We chose PacMan as the theme, therefore the name.

The libraries and projects are designed to run on an [Arduino](https://www.arduino.cc/) (tested on [Arduino Nano](http://store.arduino.cc/products/arduino-nano) and [Arduino Uno](http://store.arduino.cc/products/arduino-uno-rev3)).

The essential project is split into 4 parts:
- [arduino sketch](https://github.com/PaccerPinball/PaccerMain) - calles the libraries and specifies what should be simulated and what real input should be used
- [PaccerInput](https://github.com/PaccerPinball/PaccerInput) - gets input e.g. from sensors or simulates input and sends that data to PaccerCommon
- [PaccerCommon](https://github.com/PaccerPinball/PaccerCommon) - manages the input from PaccerInput; calculates scores etc. and sends output data (e.g. LEDs) to PaccerOutput
- [PaccerOutput](https://github.com/PaccerPinball/PaccerOutput) - manages the data from PaccerCommon and controls the outputs like the LCD or the LEDs
