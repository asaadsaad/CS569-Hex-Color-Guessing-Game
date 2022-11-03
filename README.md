# CS569-Hex Color Guessing Game
In this game users will have to guess the displayed color from 3 buttons as shown below:
<p align="center">
  <img src="./game-01.png" />
</p>
  
Once the user clicks on the answer:  
* All buttons are disabled.  
* A message is displayed with: "That's Correct!" Or "Wrong answer, the color is: #RRGGBB".  
* Display an interval countdown from 5 to 0 seconds and reset the game once it reaches 0 (Reset: pick a new color, activate buttons, remove all messages) as displayed below:  
  
<p align="center">
  <img src="./game-02-correct.png" />
  <img src="./game-03-wrong.png" />
</p>
  
## Extra requirement
Create a directive `CheatDirective`, that listens to its host element (color div) for double-click event, and displays the HEX color value as alert.
  
## Code assistance
Use the code below to generate a random HEX color value, and to pick one random value from a given array:
```javascript
  private generateRandomHexColor() {
    return '#' + (Math.random() * 0xFFFFFF << 0).toString(16).padStart(6, '0');
  }
  private getRandomItemFromArray(arr: string[]) {
    return arr[Math.floor(Math.random() * arr.length)];
  }
```
