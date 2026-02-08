# These are the blocks (for now):

---

`Collision check (string)`<br>
This block makes it easier and shorter to read a collision.  
The collision output is stored in the variable "Colliding?"  
The input is the sprite name; without it, the block will not work.

---

`New common query (any)`<br>
This is literally made for efficiency.  
It gives the variable "query" whatever value you want, so you can reuse it multiple times.

---

`Prompt (any) and save to mem`<br>
This helps with things like questionnaires or maybe simple AIs.

---

`Topdown easy controls`<br>
It isn't very efficient, but it is pretty abstract.  
It simply gives multi‑platform top‑down controls.

---

`Dist (x1) (y1) (x2) (y2)`<br>
This block uses the Pythagorean theorem to calculate the distance between two points.  
It's useful for distance between clones or pen renders.

---

# NEXT UP: COMPLEX BLOCKS

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
