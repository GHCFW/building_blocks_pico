## Activity: Play the reaction game on the Pico Board

### Step 1. Locate the board and all the components <br>

Make small groups to share the board and play the game.<br>
Your board should look something like this:

  ![Exercise 1: Board Setup](https://github.com/GHCFW/WorkshopExercise23/blob/main/images/Exercise_1_Board_Setup.jpeg)


### Step 2. Let's start by connecting the buzzer to the board. <br>
   Locate the buzzer and some jumper cables (socket-pin style cables) on your table. <br>

  &nbsp; &nbsp; ![Exercise 3: Buzzer](https://github.com/GHCFW/WorkshopExercise23/blob/main/images/Buzzer_Connections.jpeg)

  Connect the socket end of the cables to the two pins of the buzzer, and the pin ends of the jumper cables to the bread-board.

  We want to connect the buzzer to the board via: <br>
   &nbsp; &nbsp;- GND, which is connected on the bread-board via 3[abcde] <br>
   &nbsp; &nbsp;- GPIO pin 14, which is connected on the bread-board via 19 [abcde] <br>

   &nbsp; &nbsp; ![Exercise 3: Connecting Buzzer to the Board](https://github.com/GHCFW/WorkshopExercise23/blob/main/images/Buzzer_On_Board.jpeg)

   Reference <br>
      [Raspberry Pi Pico pinout diagram](https://datasheets.raspberrypi.com/pico/Pico-R3-A4-Pinout.pdf?_gl=1*1ish86u*_ga*MTc0NDY1MTcyMC4xNjk0MDQ3NTcw*_ga_22FD70LWDS*MTY5NDA1MTUwNC4yLjAuMTY5NDA1MTUwNS4wLjAuMA..)


### Step 3. Play the game!
  We have already programmed the board with the relevant code needed for this exercise. 
  Just connect the board to your laptop using the provided USB cables and start playing!!



## Additional Exercises: Play the reaction game on Wokwi
Link to Wokwi simulator for the Reaction Game:  [Wokwi Simulator - Reaction Game ](https://wokwi.com/projects/423198616631390209)

- Play the reaction game on Wokwi.
- Can you try changing the victory song for both players? Pick another song from songs library and call that in-place of the existing tune (lines 36 & 42 in main.py).
- Add another LED and use that to start the game.
