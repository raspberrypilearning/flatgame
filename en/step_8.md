## Add sound

Test it out and think of a sound that your background might make when the player sprite is walking across it. 

For example, a background of leaves might make a crunch sound. 

--- task ---
Open the Sounds tab and click 'Choose a sound'.

![Screenshot of the Sounds tab in the Scratch editor](images/sound-tab.png)
Hover over the play button to try out sounds until you find one that would work for a walking sound. Shorter sounds work best. 

--- /task ---

--- task ---
Click on the sound to select it.

![Screenshot of a sound in the Scratch editor](images/choose-sound.png)
--- /task ---

--- task ---
Edit the sound to make it softer or faster by clicking the icons in the editor.


![Screenshot of the sound editor in the Scratch editor](images/edit-sound.png)
--- /task ---

--- task ---
Add sound blocks to your code:

```blocks3
when flag clicked
go to [front v] layer
forever
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

--- task ---

**Test it again** — how does the sound work out? Is the direction okay? If you need to tweak volume or direction, you can go back and change it in your code.

--- /task ---
