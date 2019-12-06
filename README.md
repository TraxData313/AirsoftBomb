<br><br>
<b>For assistance contact antongeorgiev313@gmail.com</b>
- I'm gratefull for any feedback!
- Have fun with this project and don't forget to send me a video when you complete it!
<br><br>

# AirsoftBomb


## How to build and install it:
- Get the parts <b>(check I.)</b>
- Connect the parts <b>(check II.)</b>
- If you are not using the Arduino Online Editor, manually install the two included libraries: "Wire.h" and "LiquidCrystal_I2C.h". Installing libraries steps: https://www.arduino.cc/en/guide/libraries
- Else if you are using the Arduino Online Editor, I think those libraries come pre-installed. But let me know if you run into any trouble with this
- Upload the code to the arduino (get the code is in file bomb10.txt)
- If you get an error that the address of your LCD monitor is wrong, check out the I2C_scanner.txt file
- Use the bomb <b>(check III.)</b>
- Videos: <b>https://www.youtube.com/watch?v=Q3l8eJ0i48g&list=PLNsnBmVpuum5lYN3JTYVwlbDKrOPHElvH</b>



### I. Parts used:
- Arduino Uno
- LCD display 16x2 I2C
- Beeper + LED
- Two 4-legged buttons: B1 and B2 and two resistors (from 100 to 300 Ohms)
- Bomb wires



### II. Connections:

1. Connecting the I2C LCD display:
   1. LCD GND -> Arduino GND
   1. LCD VCC -> Arduino 5V
   1. LCD SDA -> Arduino A4
   1. LCD SCL -> Arduino A5
   1. LCD LED -> LCD Power

<b>Connecting the beeper + LED:</b>
- Beeper(+) -> Arduino 10
- LED(+) -> Arduino 10
- Beeper(-) -> Arduino GND
- LED(-) -> Arduino GND

<b>Connecting the buttons:</b>
- B1 top left leg -> Arduino 5V
- B2 top left leg -> Arduino 5V
- B1 top right leg -> Resistor (few Ohms) -> Arduino GND
- B2 top right leg -> Resistor (few Ohms) -> Arduino GND
- B1 bottom right leg -> Arduino 2
- B2 bottom right leg -> Arduino 3

<b>Connecting the bomb wires:</b>
- Arduino 12 -> Red wire -> GND
- Arduino 11 -> Black wire -> GND
- Arduino 7  -> Green wire -> GND
- Arduino 8  -> Yellow wire -> GND




### III. Usage:
- Make sure all bomb wires are connected as per the instruction above (Connecting the bomb wires)
- Start the bomb by plugging in the power (Arduino input power from 3,5 to 12V!)
- Increase the timer to desired time to detonation using B1, when ready confirm with B2
- Key will be generated, this is a defuse sequence of 3 letters where (R=RedWire,B=BlackWire...)
- Write down the sequience and press B2 to arm (start the countdown to detonation)
- Defuse the bomb by removing the bomb wires in the given sequience (key)
- Press the reset button or re-plug the power to reset



### Timers:
- The bomb will beep once per second
- When 1/3 of the time expires it will start beeping faster
- When 1/6 of the time expired it will start beeping fastest


<br><br><br>
- Not sure if I need to add this or if it ever be red, but here it it:
<p><em>Disclaimer:</em></p>
<blockquote>
<p>THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.</p>
</blockquote>
