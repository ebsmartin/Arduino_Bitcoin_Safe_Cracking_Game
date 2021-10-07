# Arduino_Bitcoin_Safe_Cracking_Game

Arduino 'Safe-Cracking' game where you try to crack into a BTC safe. Failure is not an option!

**Description of Game**

Crack the code game!

- You are attempting to crack into a device that contains sensitive cryptocurrency data.

- Have someone set a 3 digit password via the Serial Port or use the random function to generate one for you.

- Input error checking is programmed in to ensure proper input format.

- Follow the on screen instructions containing information on how to play.

- Use the rotary encoder and listen for a variation in the sound of the clicks to identify the target number and press the switch to select the chosen number.

- Once the player has chosen all three numbers, the device will either accept or decline the password

- On success, a green light will shine through the crystal and sensitive information will be displayed. WINNER!

- On failure, a red light will shine through the crystal, an alarm will sound. FAILURE!



**Description of Design Process**

Design requirements :

- Two digital or analog inputs with at most one button/switch
- Using at least two digital outputs, using at most one LED

Design Process :

- Wanted to utilize the rotary encoder

- Made me think of using a Masterlock

- Decided to design a ‘cracking the lock game’

- Use the LCD screen to display information

- Needed some auditory feedback to simulate using a Masterlock

- Utilized the piezoelectric transducer to simulate the ‘click’ of a turn

- A different click is played when the target number is passed

- Use of Serial Input and Output for user interaction

- User can set their own password or generate a random password to crack

- Alarm and light system for incorrect final guess

- Nice presentation/box


Box Design :

Using a heavy duty cardboard box with magnetic closure an LCD screen, Rotary Encoder, and Selenite crystal were embedded to create a fun  and unique presentation.


Challenges / Issues :

- The game only works on random number generation mode currently
  - This is simply due to the fact that I did not parse the user input string into three separate ints
- Screen text must fully cycle through loop before user input is read
  - This makes for some wait time after user input
- I could not get the target number to cause a unique ‘click’ when you turn to the number
  - The unique ‘click’ sound will only occur once you pass the number in either direction.
- Rotary Encoder could be better secured into box
