Components Needed:
Arduino Uno or Arduino Mega

PIR Motion Sensor (digital output)

Active Buzzer (active type)

Red LED (+ resistor recommended)

Green LED (+ resistor recommended)

Pushbutton switch

Jumper wires

Power supply (5V)

Wiring Table:
Component	Arduino Pin	Connection Details
PIR Sensor OUT	Pin 2	PIR digital output to pin 2
Active Buzzer	Pin 9	Buzzer positive to pin 9, negative to GND
Red LED (+)	Pin 6	LED anode → 1 kΩ resistor → pin 6; cathode → GND
Green LED (+)	Pin 7	LED anode → 1 kΩ resistor → pin 7; cathode → GND
Pushbutton	Pin 4	One side to pin 4; other side to GND
Power (5V)	5V	Power PIR sensor, buzzer, LEDs if needed
Ground (GND)	GND	Common ground for all components

Important Notes:
Resistors:
Always use a resistor (220Ω to 1kΩ recommended) in series with LEDs to protect them and the Arduino pins.

Pushbutton:
The code enables internal pull-up resistor, so no external pull-up resistor is needed for the button.

Power:
Use 5V supply from the Arduino for sensors and buzzer. Make sure your components support 5V.

Arduino Uno vs Mega:
Wiring is the same for both. All used pins (2,4,6,7,9) exist and work identically on Uno and Mega.

Summary Wiring Diagram (conceptual):
scss
Copy
Edit
[PIR OUT] --- Pin 2 (Arduino)

[Active Buzzer +] --- Pin 9 (Arduino)
[Active Buzzer -] --- GND

[Red LED Anode] --- 1kΩ resistor --- Pin 6 (Arduino)
[Red LED Cathode] --- GND

[Green LED Anode] --- 1kΩ resistor --- Pin 7 (Arduino)
[Green LED Cathode] --- GND

[Pushbutton] --- Pin 4 (Arduino)
[Pushbutton other side] --- GND

[5V] --- PIR VCC, buzzer VCC (if needed), LEDs power if required
[GND] --- Common ground for all
