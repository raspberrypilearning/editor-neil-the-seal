## End the game

Now end the game when Neil runs out of lives.

![stage](images/stage-sprite.png)

Click on the `Stage`.

## Step 1

Add a new script — much like your winning one — using a `forever`{:class="block3control"} loop and an `if then`{:class="block3control"} block.

When `lives`{:class="block3variables"} is less than `1` and `game over`{:class="block3variables"} is `0`, switch to your `game over` backdrop and set `game over`{:class="block3variables"} to `1`.

```blocks3
when green flag clicked
forever
if <<(lives) < (1)> and <(game over) = (0)>> then
switch backdrop to (game over v)
set [game over v] to (1)
end
end
```

## Step 2

Make a new message called `game over`.

Add a `broadcast ()`{:class="block3events"} block to the script, so the other sprites know the game has ended.

```blocks3
if <<(lives) < (1)> and <(game over) = (0)>> then
switch backdrop to (game over v)
set [game over v] to (1)
+broadcast (game over v)
end
```
