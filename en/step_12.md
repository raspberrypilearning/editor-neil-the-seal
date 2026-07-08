## Detect a win

Now check whether the town is clear, and show the `Win` backdrop when it is.

![stage](images/stage-sprite.png)

## Step 1

Make a new variable called `game over`{:class="block3variables"}, **For all sprites**, and untick its checkbox to hide it. On the Stage, add it to your setup script and set it to `0` at the start. Add a `switch backdrop to ()`{:class="block3looks"} block so the game always begins on the `Town` backdrop.

```blocks3
when green flag clicked
+switch backdrop to (Town v)
set [score v] to (0)
set [stuff to smash v] to (0)
+set [game over v] to (0)
```

## Step 2

On the Stage, add a new script to check for a win. Start with a `wait () seconds`{:class="block3control"} block for `0.2` seconds so everything can be counted first. Then use a `forever`{:class="block3control"} loop with an `if then`{:class="block3control"} block: when `stuff to smash`{:class="block3variables"} is less than `1` and `game over`{:class="block3variables"} is `0`, switch to your `Win` backdrop and set `game over`{:class="block3variables"} to `1`.

```blocks3
when green flag clicked
wait (0.2) seconds
forever
if <<(stuff to smash) < (1)> and <(game over) = (0)>> then
switch backdrop to (Win v)
set [game over v] to (1)
end
end
```

## Now run your code

Click the green flag and smash everything in town. When the last object is gone, your `Win` backdrop appears.
