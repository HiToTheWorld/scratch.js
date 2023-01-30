# sratch.js 1
Have you ever wanted to be a scripter, but only know Scratch/Block coding? If so, then you might want to check out this JavaScript extention! This extention has blocks from Scratch in JavaScript to give you an idea on how line-coding works.
**This JS extention is only available for use with HTML, JS, and CSS - Other types like Node.js will be in a future update.**

## Setting Up
This section will explain how to set up the extention.
1. Download the file "scratch.js" from [this page](https://github.com/rabitailleow/scratch.js/releases)
2. Import the file into the root directory or somewhere where you will remember it
3. On any html page you wish to have scratch on, type or paste ``<script src='scratch.js'>`` somewhere reasonable in your code and replace the src attribute with the path to your scratch.js file
4. Your all set up! Check out the [Usage](#usage) section for information on how to use the extention.

## Usage
This section will teach how to use the extention.

1. Learning the basics of JavaScript  
**If your pretty well familiar with JavaScript (or any coding language for that matter) you can skip this step.**  
- Define a varible with ``let``, ``var``, or ``const``. Each of these will change the way that the variable works. ``let`` declares a block-scoped variable meaning it only works within the current function or block of code. ``var`` declares a gloabally-scoped variable meaning you can use it anywhere in your code. ``const`` declares a variable that cannot be changed.  
- Classes can be called with just the class name, such as ``Math.PI``, or by creating a new instance of the class, such as ``const class = new Class()``.
- Unfortunetly we are unable to include booleans because it would be way too much work for users and would not work like scratch, so you need to learn ``if`` statements. Declare one like so; ``if (<boolean>) {<code>}`` Booleans can be declared as follows; ``Is equal to: ==`` ``Is greater than: >`` ``Is less than: <`` ``And: &&`` ``Or: ||`` (Or uses virtical bars (above enter/return key)) You may look up others if you need to.

2. Sprites
- Sprites can be declared with ``let <sprite name> = new Sprite("<sprite costume path>");``
- Sprite functions can be accessed through the sprite like so; ``sprite.GoTo(0, 0);``
- Sprite variables can be accessed by calling them through the sprite; ``sprite.xposition``

## Usefulness List
### Motion
``sprite.Move(10);`` Move in the direction it is facing by 10 steps  
``sprite.TurnRight(15);`` Turn 15 degrees right (clockwise)  
``sprite.TurnLeft(15);`` Turn 15 degrees left (counter-clockwise)  

``sprite.GoToRandomPosition();`` Move the sprite to a random position  
``sprite.GoTo(36, 28);`` Move the sprite to (x: 36, y: 28)  
``sprite.GlideTo(mouse, 1);`` Glide to the mouse-pointer for 1 second (you may sub out mouse for any other sprite)  
``sprite.GlideTo(0, 0, 1);`` Glide to (x: 0, y: 0) for one second  

``sprite.PointInDirection(90);`` Look 90 degrees  
``sprite.PointTowards(mouse);`` Look at mouse pointer (you may sub out mouse for any other sprite)  

``sprite.ChangeXBy(10);`` Changes the x-position by 10  
``sprite.SetXTo(36);`` Sets the x-position to 36  
``sprite.ChangeYBy(10);`` Changes the y-position by 10  
``sprite.SetYTo(28);`` Sets the y-position to 28  

``sprite.xposition`` Returns the x-position of the sprite  
``sprite.yposition`` Returns the y-position of the sprite  
``sprite.direction`` Returns the direction of the sprite  
