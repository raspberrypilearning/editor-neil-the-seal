## Give Neil a voice

Make Neil shout one of your words each time he smashes something.

![neil sprite](images/neil-sprite.png)

Click on the `Neil`{:class="block3looks"} sprite and find his movement script.

Inside the `if then`{:class="block3control"} block, add another `if then`{:class="block3control"} block that checks for the `space`{:class="block3sensing"} key.

When it's pressed, `say () for () seconds`{:class="block3looks"} a random item from your list for `0.2` seconds.

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

Click the green flag and smash away.

Neil shouts something each time, and holding down the space bar no longer clears the whole town in an instant.
