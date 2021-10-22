# Instructions

Write the script.js file to bring this piggy bank to life!

1. Whenever a user clicks one of the 4 buttons representing a deposited coin, the span element with the id "balance-amount" should have the appropriate value added to it, always rounded to 2 decimal places.

3. The ul element with the class "history" should have a new li element added for each button click as well, containing the first letter of the deposited coin (P, N, D, Q). This will show up as a grey box.

4. Each li element in the history should be removed when clicked.

5. Whenever a user clicks the balance, they should be prompted to enter a new balance. Only update the balance if the user hits OK (not Cancel), and if the entered value converts successfully to a Number. Also, round to 2 decimal places.

6. Use window.localStorage to automatically save and load the balance. This way, the 
value is retained even if the user closes the webpage.

Extra Optional Challenges:

- Make the audio element play (with the .play() method) whenever a coin is added.

- Add keypress events for each coin as an alternative to button presses.

- Save the history elements via localStorage too. Add to the HTML a new button that clears the history.

## Hint: Write helpful function(s)

Each coin button does extremely similar things. To avoid duplicating code, write a function (say, addCoin) with parameters (say, coinLetter and coinAmount) to represent the general action of adding a coin. Call this function with different parameters for each coin button click event.

## Converting to/from Number

Here are some bits that we may not have covered in class.

To convert a string into a number, use the Number function. For example:
```
let s = "1.1"
let n = Number(s); //n === 1.1
```

If the conversion is a failure, it will result in a special value called NaN. You can check this.
```
if(n !== NaN) {
    ...
}
```

To convert a Number to a string, rounded to a specific number of digits, use 
the toFixed method. For example
```
let n = 1.259;
let s = n.toFixed(2); //s === "1.26"
```




