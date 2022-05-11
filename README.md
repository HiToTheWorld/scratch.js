# JS-Scratch-Tool 1.0.0
Have you ever wanted to be a scripter, but only know Scratch/Block coding? If so, then you might want to check out this JavaScript extention! This extention has blocks from Scratch in JavaScript to give you an idea on how line-coding works.
**This JS extention is only available for use with HTML, JS, and CSS - Other types like Node.js will be in a future update.

## Setting Up
This section will explain how to set up the extention.
1. Download the file "scratchtool.js" from [this page](https://github.com/rabitailleow/JS-Scratch-Tool/releases)
2. Import the file into the directory where your main JS file is (If your somewhat familiar with directory linking, you can put it somwhere else)
3. On your main JS file, type or paste the folowing code ``import * as sct from './scratchtool.js';`` (if you placed scratchtool.js in a different directory, link it instead of ``./scratchtool.js``
4. Your all set up! Check out the [Usage](#usage) section for information on how to use the extention.

## Usage
This section will teach how to use the extention.

1. In the [Setting Up](#setting-up) section, we had you import the scratchtool.js file. on that line, after ``import * as`` is a variable name. To call the Scratch Tool, simply type that variable.
2. The variable cannot be on its own, or it will throw an error. Add the name of the function after the variable with a dot. Then add parenthasis at the end. ``sct.say();``
3. Different function call for different arguments. Add the corresponding arguments in the parenthesis, like so: ``sct.say('Hello World~');``

### Adding loops and events
Adding loops and events can be a little difficult, so here we will break it down. Although they are alike, they have some differences, so we will split them here.

#### Loops
1. Define your loop. ``sct.forever()``
2. For a repeat _ times loop, you must define the number of times. Do that first: ``sct.repeat(10, [])``
3. Define the after events. The functions must be functions in an array, like so: ``sct.forever([sct.say('Hello'), sct.say('World!')]);``

<!-- #### Events
1. Define your event with a name. We chose stage clicked ``sct.event('stage-clicked', )`` -->

To make your code a bit neater, I suggest making the functions new lines of code:

```
sct.forever([
  sct.say('Hello'), 
  sct.say('World!')
]);
```

## All Functions
Get ready! Here we've written out all of the functions added to this extention.
#### Say()
***Arguments:*** msg - Message
