## Track where Neil is

For the Ranger to chase Neil, it needs to know where Neil is.

## Step 1

Click on the `Neil`{:class="block3looks"} sprite and make two variables, `neil x`{:class="block3variables"} and `neil y`{:class="block3variables"}, both **For all sprites**. Untick both checkboxes to hide them from the player.

## Step 2

Find Neil's movement script. At the bottom of the movement code, inside the `if then`{:class="block3control"} block, set `neil x`{:class="block3variables"} and `neil y`{:class="block3variables"} to his current position.

```blocks3
if <key (right arrow v) pressed?> then
change x by (5)
point in direction (90)
next costume
end
+set [neil x v] to (x position)
+set [neil y v] to (y position)
```
