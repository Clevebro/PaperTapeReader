# Paper Tape Reader
Fork of [PaperTapeReader](https://github.com/gav-/PaperTapeReader) created by [Gavin Stewart](https://github.com/gav-). Thank you, Gavin, for the great work and inspiration.

I've created a paper tape reader based on the Arduino Nano that can be connected to a PC via USB as a fully functional device.

![Paper Tape Reader](https://raw.githubusercontent.com/Clevebro/PaperTapeReader/refs/heads/master/images/perfboard4.jpeg "Paper Tape Reader")

[![Paper_Tape_Reader_Video](https://img.youtube.com/vi/Yuy-rlHPrUo/0.jpg)](https://www.youtube.com/watch?v=Yuy-rlHPrUo)

## Modification
There are some differences from the original project:

* Arduino Nano (soldered to perfboard)
* INPUT_PULLUP mode for internal pullup resistors instead of external ones
* LED for data reading indication (blinks each time new data is available)
* Showing sync pin value for debugging purposes
* New output format (added binary format, removed octal value)
* Different order of data pins (due to soldering mistakes)

## Electrical schematic

* LED scheme
  
  ![Led_Scheme](https://raw.githubusercontent.com/Clevebro/PaperTapeReader/refs/heads/master/images/led_scheme.png "Led Scheme")

* Phototransistor scheme
  
  ![Pt_Scheme](https://raw.githubusercontent.com/Clevebro/PaperTapeReader/refs/heads/master/images/pt_scheme.png "Pt Scheme")

  > **Note:** R is a pull-up resistor in Arduino Nano (from 20 to 50 kΩ)

## Usage
Upload the firmware in the Arduino IDE and control the reader through the Serial monitor.
