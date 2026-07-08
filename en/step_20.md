## React to the end of the game

Now make the sprites respond when the game is over.

## Step 1

Click on the `Ranger`{:class="block3looks"} sprite. Add a `when I receive ()`{:class="block3events"} block for the `game over` message, and make the Ranger `say () for () seconds`{:class="block3looks"} to say "Off you go!".

```blocks3
when I receive (game over v)
say [Off you go!] for (1) seconds
```

## Step 2

Click on the `Sign`{:class="block3looks"} sprite. In the clone's `forever`{:class="block3control"} loop, add an `if then`{:class="block3control"} block that checks whether `game over`{:class="block3variables"} is `1`. If it is, `delete this clone`{:class="block3control"} to tidy up the leftover signs.

```blocks3
when I start as a clone
forever
if <<touching (Neil v)?> and <key (space v) pressed?>> then
change [score v] by (10)
change [stuff to smash v] by (-1)
delete this clone
end
+if <(game over) = (1)> then
delete this clone
end
end
```

## Now run your code

Click the green flag and let the Ranger catch Neil three times. The `game over` backdrop appears, the Ranger sends Neil back to sea, and the leftover signs disappear.
