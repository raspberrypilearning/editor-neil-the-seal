## Catch Neil

Make Neil lose a life when the Ranger catches him.

![ranger sprite](images/ranger-sprite.png)

Click on the `Ranger`{:class="block3looks"} sprite.

## Step 1

At the bottom of the `if then`{:class="block3control"} block, below the movement code, add an `if then`{:class="block3control"} block that checks if the Ranger is `touching Neil`{:class="block3sensing"}.

If so, `change lives by ()`{:class="block3variables"} by `-1` and send the Ranger back to the start.

```blocks3
if <(neil y) > (y position)> then
change y by (2)
else
change y by (-2)
end
+if <touching (Neil v)?> then
change [lives v] by (-1)
go to x: (-200) y: (140)
end
```

## Step 2

Make a new message called `got ya`, and add a `broadcast () and wait`{:class="block3events"} block inside that `if then`{:class="block3control"} block to tell the rest of the game Neil has been caught.

```blocks3
if <touching (Neil v)?> then
change [lives v] by (-1)
go to x: (-200) y: (140)
+broadcast (got ya v) and wait
end
```

You won't see the full effect yet — Neil reacts to being caught in the next step.
