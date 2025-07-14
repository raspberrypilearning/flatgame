## Moving the main sprite

Before adding the code to move the spirte, think of a sound that your background might make when the main sprite is walking accross it. 

For example, a background of leaves might make a crunch sound. 

--- task ---
On the sounds tab click choose a sound.

Hover over the play button to try out sounds until you find one that would work for a walking sound. Shorter sounds work best. 

When you have decided click on the sound to select it
--- /task ---

---task---
The sounds are quite loud.

Make the sound quieter by clicking the Softer icon
---/task---

In the code tab start to add code to animate the main sprite.

---task---
When the game starts you want the main sprite to be at the front.

Add the code:

```blocks3
+when flag clicked
+go to [front v] layer
```
---/task---


---task---
The main sprite will animate and make a sound, but it won't move. Instead, the background is moving - to make it look like main sprite move.

To animate left and right add the following code 

```blocks3
when flag clicked
go to [front v] layer
+forever
if <key (left arrow v) pressed> then
next costume
play sound (Wood Tap v) until done
end
if <key (right arrow v) pressed> then
next costume
play sound (Wood Tap v) until done
end
```
---/task---

Test your code! Press the green flag and the main sprite should move when you tap the left and right keys.

---task---
To make it look like it is moving towards each side, use a direction block.

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

Test out the directions as every sprite will be different depending on what the drawing looks like.

GIF testing direction
---/task---

---task---
```blocks3
Now use an operator block to add the up and down movements - these don't need a direction, so the code is the same for both.

when flag clicked
go to [front v] layer
forever
if <key (left arrow v) pressed> then
point in direction (130)
next costume
play sound (Wood Tap v) until done
end
if <key (right arrow v) pressed> then
point in direction (-130)
next costume
play sound (Wood Tap v) until done
end
+if <<key (up arrow v) pressed> or <key (up arrow v) pressed >> then
next costume
play sound (Wood Tap v) until done
end
```
---/task---

Test out the directions as every sprite will be different depending on what the drawing looks like.

GIF testing direction