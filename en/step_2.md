## Move Neil in every direction

## Step 1

Add another `if then`{:class="block3control"} block inside the `forever`{:class="block3control"} loop.

This time check for the `down arrow`{:class="block3sensing"} key and use `change y by ()`{:class="block3motion"} to move **Neil** down.

![Neil](images/neil-sprite.png)

```blocks3
if <key (down arrow v) pressed?> then
change y by (-5)
end
```

## Step 2

Add two more `if then`{:class="block3control"} blocks for the `left-arrow`{:class="block3motion"} and `right-arrow`{:class="block3motion"} keys.

Moving left and right changes **Neil**'s `x`{:class="block3motion"} position, so use `change x by ()`{:class="block3motion"}.

![Neil](images/neil-sprite.png)

```blocks3
if <key (left arrow v) pressed?> then
change x by (-5)
end
if <key (right arrow v) pressed?> then
change x by (5)
end
```

## Now run your code

Click the green flag and try all four arrow keys.

**Neil** moves around the town.
