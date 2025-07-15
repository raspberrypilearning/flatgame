## Challenge

Flatgames are a great way to be creative and try new things out with scratch. Try some of these challenges for next steps - and don't worry about making it neat!

Here are some ideas - have a play! What else can you add? 

### Make start text
Let people know the title of your flatgame and how to play

--- task ---
Make a paint sprite and call it "start text"
--- /task ---

--- task ---
In the costume tab, add the text you want.

Move the text so it is easy to read, somewhere near the centre.

SCREEN RECORDING
--- /task ---

--- task ---
In the start text code add the following blocks to show and hide when the flag is clicked:

```blocks3
+When flag clicked
+show
```

```blocks3
+when [any v] key pressed
+wait (0.2) seconds
+hide
```
--- /task ---

### Add more artwork sprite
Flatgames are great when they are full of art! 

--- task ---
Duplicate the thing sprite and name it artwork 2
--- /task ---

--- task ---
Upload a new costume and edit it in the same way as the artwork you made earlier.

You can think about where you want to place the new artwork sprites - are they all in a line, or spread out?
--- /task ---

### Change layer of things
It can be fun for the main spite to walk under and over the artwork, change some of the layers to do this. 

--- task ---
In the artwork sprite add the layer order block under the green flag event.

```blocks3
+go to [front v] layer
```
--- /task ---

### Animate the artwork
You could animate some of the artwork to add movement to the flatgame.

--- task ---
Ddecide on which artwork you want to animate. 

Select the chosen artwork sprite and duplicate the costume. 

Move the new costume very slightly, this will be the next sequance in the animation

SCREEN RECORD
--- /task ---


--- task ---
Make a new green flag event and add this code:

```blocks3
+when flag clicked
+forever
next costume
wait (1) seconds
```

You can change the wait time to slow down or speed up the animation 
--- /task ---