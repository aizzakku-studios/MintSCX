# These are the blocks (for now):

---

`Animate through (number) To (number) Speed (number)`<br>
What this block does is use a "() mod ()" block to switch between a set number of frames.  
(But you need to make the frames yourself.)

---

`Collision check (string)`<br>
This block makes it easier and shorter to read a collision.  
The collision output is stored in the variable "Colliding?"  
The input is the sprite name; without it, the block will not work.

---

`line (X1) (X2) (Y1) (Y2) (Color HEX) (size)`<br>
This block is very useful for rendering 2D or 3D objects easily.  
Though you might get overwhelmed with all the inputs.

---

`New common query (any)`<br>
This is literally made for efficiency.  
It gives the variable "query" whatever value you want, so you can reuse it multiple times.

---

`Play sound (string) for (number) seconds`<br>
This is pretty useful if you don't know how to use the sound editor.  
The first input needs the exact name of the sound you're trying to use.

---

`Prompt (any) and save to mem`<br>
This helps with things like questionnaires or maybe simple AIs.

---

`range (number) (number)`<br>
This returns a random value within a range.  
1st input is the middle point, and 2nd is the range.  
For example, range(0, 2) would give a random number between -2 and 2.

---

`sin wave (number) (number) (number)`<br>
This is pretty efficient and useful.  
It creates any type of sine wave based on a timer.  
1st input is the middle point, 2nd is the speed, and 3rd is the range.

---

`smooth say (any)`<br>
This is just cosmetic. It's like the text AIs show when it appears character by character.

---

`Topdown easy controls`<br>
It isn't very efficient, but it is pretty abstract.  
It simply gives multi‑platform top‑down controls.

---

`TypeOf (any)`<br>
This detects the type of the input value.  
But array‑like values will be detected as strings.

---

`Read through let (number) To let (number) Of (any)`<br>
This is pretty useful for reading values, and I even used it in part of the framework config.  
1st input is the starting letter, 2nd is the ending one, and 3rd is the text to read.

---

`Hitbox (x) (y) With properties (width) (height) Check collision with (string) Depuration? (boolean)`<br>
This is very complex.  
To keep it simple: it creates a fake hitbox and checks collisions on it.

---

`Dist (x1) (y1) (x2) (y2)`<br>
This block uses the Pythagorean theorem to calculate the distance between two points.  
It's useful for distance between clones or pen renders.

---

# NEXT UP: COMPLEX BLOCKS

---

`Interpolate (number) By (number)`<br>
This block is used to create smooth animations by interpolating a value over a specific number of frames.  
1st input is the total amount you want to interpolate.  
2nd input is how many frames the interpolation should last.

---

`Motion blur setup (number)`<br>
This block sets up the motion blur system by creating transparent clones.  
The input is how many clones will form the blur trail.  
(More clones create a smoother blur but increases cost.  
A range of 3 to 8 clones is recommended.)

---

`Motion blur (number) Latency (number) Sprite (string)`<br>
This block applies the motion blur effect to a specific sprite using the clones created in the setup.  
1st input is how transparent the blur is (0 = solid, 100 = invisible).  
2nd input is how many frames it delays between movement.  
3rd input is the name of the sprite to follow.

---

`Ftimer setup`<br>
This block sets up a fake timer by storing the current “days since 2000” value.  
It is used to create a custom timer so that you can reset the built-in one without affecting the functions that use timers.  
You must change timer manually to Ftimer in any function that uses it so it doesnt break.

---

`Ftimer ` <br>
This block calculates how many seconds have passed since the last time Ftimer setup was called.  
It subtracts the stored value from the current “days since 2000” and converts the result into seconds.

---

`Deltatime  `<br>
This block gives you the time passed between frames.  
It stores the current timer value and resets the built‑in timer, allowing you to calculate frame‑based movement or animations.

---

`Elim (number) From data`<br>
This block removes an item from a data list using its index.  
The input is a number, which represents the position of the item you want to delete.

---

`Read (number) From data`<br>
This block reads a specific item from a data list.  
The input is a number, and the output is stored in the variable “Data readed”.

---

`Save (any) To data`<br>
This block adds any value to a data list.  
Useful for storing text, numbers, or any other type of value.

---

`Find (any) in data`<br>
This block searches the data list for a specific value.  
It returns the index (number) of the first matching item.  
If the value is not found, it returns 0.

Useful for inventories, searching text, or checking if something already exists in your data.

---

`Count occurrences of (any) in data`<br>
This block counts how many times a specific value appears in the data list.  
It returns a number representing the total matches.

Great for statistics, repeated items, or validating user input.

---

`Is (input) between (min) and (max)?`<br>
This block checks if a value is inside a numeric range.  
It returns true if the input is greater than or equal to min and less than or equal to max.  
Otherwise, it returns false.

Useful for validating values, clamping logic, or checking boundaries in games.

---

`Toggle bool`<br>
This block flips a boolean variable between true and false.  
If the value was true, it becomes false.  
If it was false, it becomes true.

Great for switches, states, UI toggles, and simple logic systems.

---

`Single out (data)`<br>
This block removes duplicate values of the data you want in the data list.  
After running it, the list will contain only unique items, keeping the first occurrence of each one.

Useful for cleaning data, inventories, or avoiding repeated entries.

---

`Pulse to (size) speed (speed)`<br>
This block smoothly scales a sprite up to a target size and then returns it back to normal, creating a “pulse” effect.  
The speed controls how fast the pulse animation happens. (less speed = less iterations)

Perfect for UI feedback, hit effects, attention grabbers, or animated buttons.

---

`Tween (angle) (speed) (cw or ccw)`<br>
This block rotates the sprite smoothly toward a target angle.  
You can choose the direction: cw (clockwise) or ccw (counter‑clockwise).  
The speed determines how fast the rotation interpolates. (less speed = less iterations)

Useful for animations, aiming systems, transitions, and polished movement.

---
