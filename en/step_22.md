## Give Neil a voice

At the moment, the player can just hold down the space bar to smash everything at once. Add a short delay — and give Neil something to say each time he smashes.

## Step 1

Make a new list called `neil's words`{:class="block3variables"}, **For all sprites**. Using the list on the Stage, click the `+` to add a few things for Neil to shout — as many as you like, and anything you want! Then untick the list's checkbox to hide it from the player.

## Step 2

Click on the `Neil`{:class="block3looks"} sprite and find his movement script. Inside the `if then`{:class="block3control"} block, add another `if then`{:class="block3control"} block that checks for the `space`{:class="block3sensing"} key. When it's pressed, `say () for () seconds`{:class="block3looks"} a random item from your list for `0.2` seconds.

```blocks3
+if <key (space v) pressed?> then
say (item (pick random (1) to (length of [neil's words v])) of [neil's words v]) for (0.2) seconds
end
set [neil x v] to (x position)
set [neil y v] to (y position)
```

## Tip

Using `length of ()`{:class="block3variables"} means Neil will always pick from however many things you added to the list.

## Now run your code

Click the green flag and smash away. Neil shouts something each time, and holding down the space bar no longer clears the whole town in an instant.
