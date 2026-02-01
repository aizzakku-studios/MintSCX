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
