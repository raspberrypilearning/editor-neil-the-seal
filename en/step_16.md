## Make the Ranger chase Neil

Now use Neil's position to move the Ranger towards him.

![ranger sprite](images/ranger-sprite.png)

Click on the `Ranger`{:class="block3looks"} sprite.

## Step 1

Inside the `if then`{:class="block3control"} block, add an `if then else`{:class="block3control"} block: if `neil x`{:class="block3variables"} is greater than the Ranger's `x position`{:class="block3motion"}, `change x by ()`{:class="block3motion"} to move right, otherwise move left.

```blocks3
if <(game over) = (0)> then
+if <(neil x) > (x position)> then
change x by (2)
else
change x by (-2)
end
end
```

## Step 2

Now do the same for Neil's y position, so the Ranger follows him up and down as well.

```blocks3
if <(game over) = (0)> then
if <(neil x) > (x position)> then
change x by (2)
else
change x by (-2)
end
+if <(neil y) > (y position)> then
change y by (2)
else
change y by (-2)
end
end
```

## Now run your code

Click the green flag.

The Ranger now chases Neil wherever he waddles.
