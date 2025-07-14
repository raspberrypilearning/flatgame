## Adding things!

In this step you can get creative adding textures, drawings, or any things that you want to complete your flatgame.

--- task ---
Upload a new sprite and name it "thing 1"

Use one of your drawings or a photo you have taken
--- /task ---


---task---
Remove any background you don't want - this has a collage effect so don't be too neat!
---/task---

---task---
Use the select tool and line up with the centre
---/task---

---task---
Convert to Vector
---/task---

---task---
Resize and position the image. You can zoom in and out with the - and +. 

For best resaults position the thing sprite at the edges of the XXXNAME of paint window, so that your main sprite can explore further.

If you move the image out of the XXXNAME of paint window, make sure a small bit of it is still showing otherwise it will be hard to reposition if you want to edit later.
---/task---


---task---
Add text

This can be playful. You could:

- write a few words about why you chose this
- describe it
- repeat and overlap words

Change the colours, size and position of the text.

Again, if you move the text out of the XXXNAME of paint window, make sure a small bit of it is still showing otherwise it will be hard to reposition if you want to edit later.
---/task---

---task---
Add code to move the thing sprite. This will be very similar to the background sprite code, as they move around in the same way.

```blocks3
+when flag clicked
+forever
set x to (move x)
set y to (move y)
if<key (left arrow v) pressed>then
change [move x v] by (1)
end
if<key (right arrow v) pressed>then
change [move x v] by (-1)
end
if<key (up arrow v) pressed>then
change [move y v] by (-1)
end
if<key (down arrow v) pressed>then
change [move y v] by (1)
end
```
---/task---

Test it out! Your thing sprite should move around in with the background.