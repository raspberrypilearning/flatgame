## Scrolling 

*not edited vid yet*

To make a scrolling effect, the background sprite moves on the x and y axis when the keys are pressed,

--- task ---
Add these two blocks to the background code. They set the *move x* and *move y* `variables`{:class="block3variables"} to 0.

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

--- task ---
Add a loop and set the x and y values of the background sprite to the *move x* and *move y* `variables`{:class="block3variables"}.

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
--- /task ---


--- task ---
Use `if`{:class="block3control"} blocks to sense when each arrow XXXkey is pressed. For each arrow key add a `change`{:class="block3variables"} block this will change move x or move y by 1 or -1 to move the background.

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
--- /task ---

Test it out! The background sprite should move around when you press the arrow keys. If it seems a bit slow you can increase the move numbers to make it faster.