## Scrolling 

To make a scrolling effect, the background sprite moves on the x and y axis when the keys are pressed,

--- task ---
Add these blocks to make sure we start at 0

```blocks3
when flag clicked
switch costume to (zoom v)
set size to [400]%
switch costume to (background v)
go to [back v] layer
+ set [move x v] to (0)
+ set [move y v] to (0)
```
--- /task ---



---task---
Set the x and y values of the sprite to a variable, so that we can change it

```blocks3
when flag clicked
switch costume to (zoom v)
set size to [400]%
switch costume to (background v)
go to [back v] layer
set [move x v] to (0)
set [move y v] to (0)
+forever
set x to (move x)
set y to (move y)
```
---/task---


---task---
Use if blocks to sense which key is pressed and change the move x or move y by 1 in all directions.

This is the code to add

```blocks3
when flag clicked
switch costume to (zoom v)
set size to [400]%
switch costume to (background v)
go to [back v] layer
set [move x v] to (0)
set [move y v] to (0)
forever
set x to (move x)
set y to (move y)
+if<key (left arrow v) pressed>then
change [move x v] by (1)
end
+if<key (right arrow v) pressed>then
change [move x v] by (-1)
end
+if<key (up arrow v) pressed>then
change [move y v] by (-1)
end
+if<key (down arrow v) pressed>then
change [move y v] by (1)
end
```
---/task---

Test it out! The background sprite should move around when you press the arrow keys.