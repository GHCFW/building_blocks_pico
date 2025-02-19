## Activity: Blink an LED using Wokwi Simulator for Raspberry Pi Pico


### Exercise 1. Open the Wokwi project and run the code <br>
- Click on the following link to open the project in the Wokwi simulator: [Wokwi Simulator Exercise - Blink a LED ](https://wokwi.com/projects/423295153155911681).

- Start by running this simulation. You should see a print in the console: `Hello, Pi Pico!`


### Exercise 2. Setup the circuit by adding a LED & a resistor to the Pico board <br>

- Add a LED and a resistor (1 kOhm) to your design. <br>
- Connect one end of the LED terminal (A- Anode) to any GP (general-purpose) pin provided on the board. Connect a resistor to the other end of the LED terminal (C- Cathode). <br>
- Connect the other end of the resistor to any GND pin on the board.

  ![Exercise 2: LED Setup](https://github.com/GHCFW/building_blocks_pico/blob/main/images/led_resistor_pico.png)


### Exercise 3. Configure the LED Pin <br>

- Configure the LED pin as an output pin. <br>
- In MicroPython, the Pin module is used to control General-Purpose Input/Output (GPIO) pins on the Raspberry Pi Pico. To use it, we need to import the Pin class from the machine module. <br>

```
from machine import Pin
```

- In the example above, the LED is connected to GPIO3 on the board. You can configure GPIO3 as an output using the Pin class from the Raspberry Pi Pico SDK:
```
led = Pin(3, Pin.OUT)
```

- Here, `Pin(<pin number>, <direction>)` sets the specified GPIO pin as input or output based on the given direction. 

`led` is now an object that can be used to turn the pin ON and OFF using `.value(1)` and `.value(0)`, respectively.

Note: Since python executes the code sequentially, Pin class must be imported before it is used.

### Exercise 4. Program the LED to turn ON<br>

Use the `value()` method to set the LED pin to 1, which turns the LED ON.

```
led.value(1)
```


### Exercise 4. Program the LED to turn OFF <br>

Use the `value()` method to set the LED pin to 0, which turns the LED OFF.

```
led.value(0)
```


### Exercise 5. Make the LED blink <br>

To make the LED blink, add a delay after turning it on and off. <br>

Use the method `time.sleep(<value in seconds>)` to pause the execution for the specified duration. <br>
`sleep()` is a function available from the `time` module. `time` module should be imported prior to using `time.sleep()` as Python executes code sequentially.

Import the time module as:
```
import time
```

Add some delay after turning the LED ON and OFF, like this:
```
led.value(1)
time.sleep(0.3)
led.value(0)
time.sleep(0.3)
```

Try different sleep values and see what happens!



### Exercise 6. Make the LED blink multiple times <br>

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

In this example, the while loop continues running as long as `blink_count` is greater than 0. Each time the loop runs, the LED blinks once, and the counter decreases until it reaches zero.

#### Understanding Indentation in Python
Python relies on indentation to identify which lines of code belong together. All statements inside the while loop must be indented to indicate that they belong to the loop. Improper indentation can cause errors or unexpected behavior.


#### Try This!
- Print blink_count inside the loop to observe how it changes. <br>
- Modify the code to make the LED blink infinitely! <br>
- Change the blink speed by adjusting the time.sleep() values.




<br>

# Answer Key
  
   https://wokwi.com/projects/423295100321284097  

    
<br>
