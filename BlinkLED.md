## Activity: Blink an LED using Wokwi Simulator for Raspberry Pi Pico


### Exercise 1. Open the Wokwi project and run the code <br>
- Click on the following link to open your project in the Wokwi simulator: [Wokwi Simulator Exercise - Blink a LED ](https://wokwi.com/projects/423295153155911681).

- Start by running this simulation. You should see a print in the console: Hello, Pi Pico!


### Exercise 2. Setup the circuit by adding a LED & a resistor to the Pico board <br>

- Add a LED and a resistor (1 kOhm) to your design. <br>
- Connect one end of the LED terminal (A- Anode) to any GP (general-purpose) pins provided on the board. Connect a resistor to the other end of the LED terminal (C- Cathode). <br>
- Connect the other end of the resistor to any GND pin on the board.

  ![Exercise 2: LED Setup](https://github.com/GHCFW/building_blocks_pico/blob/main/images/led_resistor_pico.png)


### Exercise 3. Code: Configure the LED Pin <br>

Configure the LED pin as an output pin. In the below example, LED is connected to GP3 pin on the board and that is configured as an output pin using the `Pin(<Pin number>, <Direction>)` module provided by Raspberry Pi Pico SDK
```
led = Pin(3, Pin.OUT)
```
Note: Pin module is imported using the following code:

```
from machine import Pin
```

### Exercise 4. Code: Program the LED to turn ON<br>

Use the method 'value(<0 or 1>)' to assign 1 to the given led pin. 1 -> Power on the LED!
```
led.value(1)
```


### Exercise 4. Code: Program the LED to turn OFF <br>

Use the method 'value(<0 or 1>)' to assign 0 to the given led pin. 0 -> Power off the LED!

```
led.value(0)
```


### Exercise 5. Code: Make the LED blink <br>

Add some time after turning on and turning off the LED to see the LED blink. 
Use the method 'time.sleep(<value in seconds>)' to add some delay

```
led.value(1)
time.sleep(0.3)
led.value(0)
time.sleep(0.3)
```

Try different sleep values and see what happens!

Note: Sleep module is imported using the time library

```
import time
```


### Exercise 6. Code: Make the LED blink multiple times <br>

Use a `while` loop to abstract your code and blink the LED multiple times. The example below blinks the LED 5 times.

```
blink_count = 5

while(blink_count > 0):
    led.value(1)
    time.sleep(0.3)
    led.value(0)
    time.sleep(0.3)
    blink_count = blink_count - 1
```

In the example above, the while loop is designed to blink the LED 5 times. Each statement inside the loop must be indented to show that they belong to the loop, meaning they should repeat each time the loop runs.

Note: Python relies on indentation to identify which lines of code belong together. Without proper indentation, Python  (or MicroPython) will not be able to understand what code is part of the loop or function. This will result in program to behave unpredictably.

- Can you print the blink_count?
- Can you try making the LED blink infinitely?

<br>

# Answer Key
  
   https://wokwi.com/projects/423295100321284097  

    
<br>
