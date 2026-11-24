## Give Neil a voice

## Step 1

![Neil](images/neil-sprite.png)

Make a list called `neil's words`{:class="block3variables"}, **For all sprites**.

Use the **+** on the list monitor to add a few things to shout, then untick the list's checkbox to hide it.

## Step 2

Inside `if game over = 0 then`{:class="block3control"} in **Neil**'s movement script, add an `if then`{:class="block3control"} block that checks for the `space`{:class="block3sensing"} key.

Use `say () for () seconds`{:class="block3looks"} to say a random list item for `0.2`{:class="block3looks"} seconds.

![Neil](images/neil-sprite.png)

```blocks3
when green flag clicked
forever
if <(game over) = (0)> then
if <key (up arrow v) pressed?> then
change y by (5)
next costume
end
if <key (down arrow v) pressed?> then
change y by (-5)
next costume
end
if <key (left arrow v) pressed?> then
change x by (-5)
point in direction (-90)
next costume
end
if <key (right arrow v) pressed?> then
change x by (5)
point in direction (90)
next costume
end
+if <key (space v) pressed?> then
say (item (pick random (1) to (length of [neil's words v])) of [neil's words v]) for (0.2) seconds
end
set [neil x v] to (x position)
set [neil y v] to (y position)
end
end
```

Using `length of ()`{:class="block3variables"} includes every item in your list, even if you add more words.

## Now run your code

Click the green flag, move **Neil**, and press the space bar. He shouts a random item from your list, with a short pause in his movement while he speaks.
