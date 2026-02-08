# These are the blocks (for now)

---

`Animate through (number) To (number) Speed (number)`<br>
What this block does is use a "() mod ()" block to switch between a set number of frames.  
(But you need to make the frames yourself.)

---

`line (X1) (X2) (Y1) (Y2) (Color HEX) (size)`<br>
This block is very useful for rendering 2D or 3D objects easily.  
Though you might get overwhelmed with all the inputs.

---

`Play sound (string) for (number) seconds`<br>
This is pretty useful if you don't know how to use the sound editor.  
The first input needs the exact name of the sound you're trying to use.

---

`sin wave (number) (number) (number)`<br>
This is pretty efficient and useful.  
It creates any type of sine wave based on a timer.  
1st input is the middle point, 2nd is the speed, and 3rd is the range.

---

`smooth say (any)`<br>
This is just cosmetic. It's like the text AIs show when it appears character by character.

---

`Hitbox (x) (y) With properties (width) (height) Check collision with (string) Depuration? (boolean)`<br>
This is very complex.  
To keep it simple: it creates a fake hitbox and checks collisions on it.

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
