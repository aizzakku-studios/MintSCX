# FIRST TUTORIAL

The first thing we're making is a topdown movement system.
First, create a sprite called "Player".
Drag the blocks "Topdown easy controls" and "Collision check" to the new sprite.
Set up this:

`SCX & Scratch`<br>
`when flag clicked`<br> `forever`<br> `Topdown easy controls`

Next, create a new sprite called "Walls".
Center it at x: 0, y: 0 and give it a costume that represents your walls.

Then, go back to the Player sprite and add collision detection:

`SCX & Scratch`<br>
`when flag clicked`<br> `forever`<br> `Topdown easy controls`<br> `Collision check [Walls]`<br> `if <(Colliding?) = 1> then`<br> `move (-5) steps`

Now you have a functioning topdown movement system in just a few blocks.
Make sure your Player sprite has a costume so collisions work correctly.

# SECOND TUTORIAL

Let's make a sine wave.  
First, create a sprite called "sine wave".  
Drag the "sin wave" block definition into that sprite.  
Set up this:

`SCX & Scratch`<br>
`when flag clicked`<br>
`forever`<br>
`Sin wave (0, 500, 25)`<br>
`set y to (Sine)`

Now we want another one.  
Copy the blocks and switch them like this:

`SCX & Scratch`<br>
`when flag clicked`<br>
`forever`<br>
`Sin wave (0, 500, 25)`<br>
`set y to (Sine)`<br>
`Sin wave (0, 250, 50)`<br>
`set x to (Sine)`

Now add the pen extension.  
Then set up this:

`SCX & Scratch`<br>
`when flag clicked`<br>
`pen up`<br>
`clear`<br>
`set pen color to [black]`<br>
`forever`<br>
`pen down`<br>
`Sin wave (0, 500, 25)`<br>
`set y to (Sine)`<br>
`Sin wave (0, 250, 50)`<br>
`set x to (Sine)`<br>
`pen up`

Now you have a sine wave displayer.

# THIRD TUTORIAL

This is a small project, but it’s cool to have.  
Make a new sprite called whatever you want.  
Drag the blocks "Prompt and save to mem", "TypeOf" and "Smooth say" to that sprite.  
Set up this:

`SCX & Scratch`<br>
`when flag clicked`<br>
`delete all of [Pmem]`<br>
`Prompt Input: And save to mem`<br>
`TypeOf item (1) of [Pmem]`<br>
`Smooth say (Type)`

This can tell you the type of any value.  
Minus things like arrays or tuples.

# FOURTH TUTORIAL

I'm sure that data management will be pretty useful in any app.  
That's why today we are gonna use the three useful functions to manage data in MintSCX.  
First, we are gonna add some data:

`SCX & Scratch`<br>
`when flag clicked`<br>
`Save (apple) to data`<br>
`Save (banana) to data`<br>
`Save (orange) to data`

Now that we have some data, let's read a specific item.  
For example, let's read the second element:

`SCX & Scratch`<br>
`Read (2) From data`<br>
`smooth say (Data readed)`

This will say banana, since it's the second item in the list.

Next, let's delete an item from the data list.  
In this example, we will remove the first element:

`SCX & Scratch`<br>
`Elim (1) From data`

Now your data list only contains banana and orange.

You can combine these three functions to build things like inventories, task lists, save systems, or any kind of structured data.

---
