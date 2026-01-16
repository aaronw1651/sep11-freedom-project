# Mastering Visual Logic in Kaboom.js
#### 1/16/26

##### Over the past few weeks, Luciano and I have been diving deep into game development for our project, specifically focusing on creating reactive visuals with the Kaboom.js library. Our goal has been to understand how code translate players actions - like making a mistake - into a visual representation on the screen.

## Creating Visual state
##### In a game like Hangman, the visuals must react to the player's errors. We have ben working on a script that draws a oink character piece by piece based on the game's current state.
* The state : we use a variable let mistake +0 to track wrong guesses.
* Drawing Array: instead of long"if: statements, we use an array of functions called hangmanParts.
* Kaboom.js Primitives; Each function uses tools like drawCircle() and drawLine().
* The Render Loop: Using the onDraw hook, a for loops fires drawing functions based on the current mistake count.


[Previous](entry01.md) | [Next](entry03.md)

[Home](../README.md)
