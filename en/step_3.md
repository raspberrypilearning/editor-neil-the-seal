## Make Neil face the right way

Right now Neil always faces the same way.

Make him face the way he walks by adding a `point in direction ()`{:class="block3motion"} block to the `left arrow`{:class="block3sensing"} and `right arrow`{:class="block3sensing"} `if then`{:class="block3control"} blocks — `-90` to face left, and `90` to face right.

![neil sprite](images/neil-sprite.png)

```blocks3
if <key (left arrow v) pressed?> then
change x by (-5)
+point in direction (-90)
end
if <key (right arrow v) pressed?> then
change x by (5)
+point in direction (90)
end
```

## Now run your code

Click the green flag and move Neil left and right.

He turns to face the way he's walking.
