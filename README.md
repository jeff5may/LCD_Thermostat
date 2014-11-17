LCD_Thermostat
==============

The beginning of a general-purpose heat pump controller.

I am working on this project as a group effort on ecorenovator forum to develop a general purpose heat pump controller.
This initial sketch is meant to run as a wall thermostat or in a "PTAC" type unit. It runs on an arduino Uno R3 controller, 
and connects to various sensors and relays to do its job. These relays are not to be powered by the arduino board, they must be 
isolated from drawing current from the board.

Pin assignment is as follows:
A0: Keypad
A1,A2: analog 10k NTC thermistor sensors (not yet coded)
A3,A4,A5: open

D0,D1: serial comms
D2: "W" output (default: aux heat/outdoor fan motor)
D3: "Y" output (default: compressor contactor)
D4-D10: LCD shield
D11:"O" output (default: reversing valve, energized in cooling mode)
D12:"G" output (default: indoor fan motor)
D13: 1-wire bus
