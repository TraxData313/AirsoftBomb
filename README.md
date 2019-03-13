# AirsoftBomb


README:
- Get the parts (check I.)
- Connect the parts (check II.)
- Upload the code to the arduino (get the code is in file bomb10.txt)
- Use the bomb (check III.)



I. Parts used:
- Arduino Uno
- LCD display 16x2 I2C
- Beeper + LED
- Two 4-legged buttons: B1 and B2 and two resistors
- Bomb wires



II. Connections:

Conncting the display:
LCD GND -> Arduino GND
LCD VCC -> Arduino 5V
LCD SDA -> Arduino A4
LCD SCL -> Arduino A5
LCD LED -> LCD Power

Connecting the beeper + LED:
Beeper(+) -> Arduino 10
LED(+) -> Arduino 10
Beeper(-) -> Arduino GND
LED(-) -> Arduino GND

Connecting the buttons:
B1 top left leg -> Arduino 5V
B2 top left leg -> Arduino 5V
B1 top right leg -> Resistor (few Ohms) -> Arduino GND
B2 top right leg -> Resistor (few Ohms) -> Arduino GND
B1 bottom right leg -> Arduino 2
B2 bottom right leg -> Arduino 3

Connecting the bomb wires:
Arduino 12 -> Red wire -> GND
Arduino 11 -> Black wire -> GND
Arduino 7  -> Green wire -> GND
Arduino 8  -> Yellow wire -> GND




III. Usage:
- Make sure all bomb wires are connected as per the instruction above (Connecting the bomb wires)
- Start the bomb by plugging in the power (Arduino input power from 3,5 to 12V!)
- Increase the timer to desired time to detonation using B1, when ready confirm with B2
- Key will be generated, this is a defuse sequence of 3 letters where (R=RedWire,B=BlackWire...)
- Write down the sequience and press B2 to arm (start the countdown to detonation)
- Defuse the bomb by removing the bomb wires in the given sequience (key)
- Press the reset button or re-plug the power to reset



Timers:
- The bomb will beep once per second
- When 1/3 of the time expires it will start beeping faster
- When 1/6 of the time expired it will start beeping fastest


For more assistance contact antongeorgiev313@gmail.com
