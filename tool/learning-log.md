# Tool Learning Log

## Tool: **X**

## Project: **X**

---

### 10/6/25:
*
<ul>
<li>push() Method: Adds one or more elements to the end of an array.</li>

<li>pop() Method: Removes the last element from an array and returns that element.</li>

<li>shift() Method: Removes the first element from an array and returns that element.</li>

<li>unshift() Method: Adds one or more elements to the beginning of an array.</li>
</ul>
<h1>Storing and Nesting Variables</h1>
<h3>An array is a data structure that lets you store an ordered collection of multiple values in a single variable. For example, let colors = ["red", "green", "blue"];.</h3>

<h3>You can create a multi-dimensional array by placing an array inside another array. This is useful for representing grids or tables. For example, let matrix = [[1, 2], [3, 4]];.</h3>


### 11/5/25:
* #### Kaboom.js Tutorial:[https://youtu.be/iRXI6ThRJvM?si=dIbD3TvGnU-gIsS0]
### Things i tried

* #### Setup and Code Separation: I started by initializing a single Kaboom instance and exporting it as"k" from its own file. This allowed me to import "k" and define scenes as pure functions in separate files.

* #### Animations: This took a bit more time. I loaded the tilemap.png using k.loadSprite , defining the slices as 20x20 . I managed to define the idle and run animations using the from and to properties. I was able to trigger the run animation on keyPress and switch back to idle on keyRelease.

### Challenges & Aha moments

#### The biggest challenge was loading the sprite sheet and figuring out the frame numbers for the animations. The video's creator mentioned the documentation for defining animations might be slightly outdated, recommending the from and to object structure instead of an array of frame numbers. I had to carefully count the rows and columns to find the right indices (like 300 for the idle frame) to define my sprites and animations.

#### The major A-ha Moment came with understanding the functional component pattern. The creator stressed that "everything is just all your entities... you just have components and you just put them in an array". This is so much simpler than managing large classes, as in other game engines. For example, the simple solution for flipping the player sprite using player.scale.x = -1 when moving left was a good and easy to implement.

### Questions I have

* #### The video shows how to load a single tilemap for sprites, but I'm unsure about the best practices for managing a large number of diverse assets ( separate sprite sheets, sound effects, music) without having a cluttered main.js file. (due to what i want to do with my project).

### What im going to do next

#### Plan to use k.addLevel with an array of strings to build a basic platformer map. This will allow me to immediately test out more advanced player movement, including using k.keyDown for continuous left/right movement and k.keyPress for a single-press jump [23:00].




<!--
* Links you used today (websites, videos, etc)
* Things you tried, progress you made, etc
* Challenges, a-ha moments, etc
* Questions you still have
* What you're going to try next
-->
