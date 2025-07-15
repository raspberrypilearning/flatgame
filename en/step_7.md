## Moving the main sprite

The main sprite will animate to look like it is moving, but it is actually the background that is moving, which you set up earlier.



--- task ---
When the game starts you want the main sprite to be at the front. 

In the main sprite code tab, add a layer block when the flag is clicked:

```blocks3
+when flag clicked
+go to [front v] layer
```
--- /task ---

--- task ---

--- task ---
To make it look like it is moving towards each side, use a direction block when the arrow keys are pressed.

```blocks3
when flag clicked
go to [front v] layer
forever
if <key (left arrow v) pressed> then
+point in direction (130)
next costume
play sound (Wood Tap v) until done
end
if <key (right arrow v) pressed> then
+point in direction (-130)
next costume
play sound (Wood Tap v) until done
end
```
--- /task ---

Test your code! Press the green flag and the main sprite should move when you use the left and right keys.

--- task ---
Your direction might be different - test out a few angles with the direction block until it looks like your srite is facing the right way as every sprite will be different depending on what the drawing looks like.

GIF testing direction
--- /task ---

--- task ---
```blocks3
Now use an operator block to add the up and down keys. These don't need a direction, so the code is the same for both up and down.

when flag clicked
go to [front v] layer
forever
if <key (left arrow v) pressed> then
point in direction (130)
next costume
end
if <key (right arrow v) pressed> then
point in direction (-130)
next costume
end
+if <<key (up arrow v) pressed> or <key (up arrow v) pressed >> then
next costume
end
```
--- /task ---

Add sound to make it look a bit more life like. Test it out again and think of a sound that your background might make when the main sprite is walking accross it. 

For example, a background of leaves might make a crunch sound. 

--- task ---
On the sounds tab click choose a sound.

Hover over the play button to try out sounds until you find one that would work for a walking sound. Shorter sounds work best. 

When you have decided click on the sound to select it

IMAGE
--- /task ---

--- task ---
The sounds are quite loud.

Make the sound quieter by clicking the Softer icon

IMAGE
--- /task ---

--- task ---
Add sound blocks to your code:

```blocks3
when flag clicked
go to [front v] layer
+forever
if <key (left arrow v) pressed> then
next costume
+play sound (Wood Tap v) until done
end
if <key (right arrow v) pressed> then
next costume
+play sound (Wood Tap v) until done
end
if <<key (up arrow v) pressed> or <key (up arrow v) pressed >> then
next costume
+play sound (Wood Tap v) until done
end
```
--- /task ---

Test it again - how does the sound work out? Is the direction ok? If you need to tweak volume or direction you can go back and change it in your code.


