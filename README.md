# CS569-Hex Color Guessing Game
In this game users will have to guess the displayed color from 3 buttons as shown below:
<p align="center">
  <img src="./game-01.png" />
</p>
Once the user click on the answer:
* All buttons are disabled
* If the answer is correct they see: "That's Correct!" Or "Wrong answer, the color is: #RRGGBB"
* Displayed an interval countdown from 5 to 0 seconds and reset the game (pick a new color, activate buttons, remove all messages) as displayed below:
<p align="center">
  <img src="./game-02-correct.png" />
  <img src="./game-03-wrong.png" />
</p>

## Extra requirements
Create a directive `CheatDirective`, that listens to its host element (color div) for double-click event, and displays the hex color value as alert.
