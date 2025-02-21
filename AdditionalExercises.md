## Additional Exercises: Blink LED

- Can you make the LED blink multiple times? <br>
  - Print the blink_count and observe how it changes. <br>
  - Change the blink speed by adjusting the time.sleep() values.
  - Make the LED blink in a pattern (e.g., short-short-long blinks like Morse code). <br>
- Add more LEDs to your circuit and make them blink. <br>
  - Make them blink in a pattern, one after the other! <br>
- Make the on-board LED blink. Hint: Use pin 25 to configure the onboard LED! <br>
- Use `led.toggle()` instead of `led.value()` to change the LED state.  <br>
- Update the code to use a for loop, instead of a while loop. Do you notice any differences? <br>
- Make the LED blink infinitely! <br>
- Use `input()` to ask the user how many times they want the LED to blink. Let them enter a number to control the number of blinks dynamically. <br>
- Create a function called `blink_led()` and encapsulate the related code within this function. What are the benefits of structuring your code this way? <br>
- Add a button to your circuit. The LED should blink only after the user presses the button. The button will act as a trigger to start the blinking process. <br>
- What happens if you switch the LED terminals A & C (connect pin A (anode) to GND and  pin C (cathode) to a GP pin)? <br>




## Play the reaction game on Wokwi

Link to Wokwi simulator for the Reaction Game:  [Wokwi Simulator - Reaction Game ](https://wokwi.com/projects/423387272779429889)

- Play the reaction game on Wokwi.
- Can you try changing the victory song for both players? Pick another song from songs library and call that in-place of the existing tunes (hint: look at lines 36 & 42 in main.py).
- Add another LED and use that to start the game.

## Additional Learning Resources

-  You bought a new Pico board. What next? See how to flash MicroPython and setup the board [here](https://github.com/GHCFW/LevelUpLab2023/blob/main/Getting_started_on_pico.md).
-  [Additional Wokwi Pico Projects to explore](https://wokwi.com/pi-pico)
-  [Raspbery Pi Pico Datasheet](https://datasheets.raspberrypi.com/rp2040/rp2040-datasheet.pdf)
-  [Raspberry Pi Pico SDK](https://github.com/raspberrypi/pico-sdk)
-  [Raspberry Pi Pico SDK in C](https://datasheets.raspberrypi.com/pico/raspberry-pi-pico-c-sdk.pdf)
-  [Pico Examples on Github](https://github.com/raspberrypi/pico-examples)

