## Catch Neil

Now make Neil lose a life when the Ranger catches him.

## Step 1

Click on the `Ranger`{:class="block3looks"} sprite. At the bottom of the `if then`{:class="block3control"} block, below the movement code, add an `if then`{:class="block3control"} block that checks if the Ranger is `touching Neil`{:class="block3sensing"}. If so, `change lives by ()`{:class="block3variables"} by `-1` and send the Ranger back to the start.

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

## Step 3

Click on the `Neil`{:class="block3looks"} sprite. Add a `when I receive ()`{:class="block3events"} block for the `got ya` message. Send Neil back to his starting position, then make him `say () for () seconds`{:class="block3looks"} to say "Hey!".

```blocks3
when I receive (got ya v)
go to x: (0) y: (-40)
say [Hey!] for (0.6) seconds
```

## Now run your code

Click the green flag and let the Ranger catch Neil. Neil says "Hey!", pops back to the start, and loses a life.
