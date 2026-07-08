## Give Neil lives

Neil needs some lives to lose when the Ranger catches him.

![stage](images/stage-sprite.png)

Click on the `Stage`.

Make a new variable called `lives`{:class="block3variables"}, **For all sprites**, and tick its checkbox so the player can see it.

Add it to your setup script and set `lives`{:class="block3variables"} to `3` at the start.

```blocks3
when green flag clicked
switch backdrop to (Town v)
set [score v] to (0)
set [stuff to smash v] to (0)
set [game over v] to (0)
+set [lives v] to (3)
```

You'll see `lives` set to `3`, but Neil can't lose one yet — you'll add that next.
