## Stop Neil when the game ends

When the game is over, **Neil** should stop moving.

Wrap all of his movement code in an `if then`{:class="block3control"} block that only runs while `game over`{:class="block3variables"} equals `0`{:class="block3operators"}.

![Neil](images/neil-sprite.png)

```blocks3
when green flag clicked
forever
+if <(game over) = (0)> then
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
end
end
```

## Now run your code

Click the green flag and smash everything.

When the last object is gone, your `Win`{:class="block3looks"} backdrop appears and **Neil** stops moving.
