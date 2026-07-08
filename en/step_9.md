## Set up the score

Now reward the player for smashing things, and keep track of how much is left.

![stage](images/stage-sprite.png)

Click on the `Stage`.

Make two variables, `score`{:class="block3variables"} and `stuff to smash`{:class="block3variables"}, both **For all sprites**.

Tick `score`{:class="block3variables"} so the player can see it, and untick `stuff to smash`{:class="block3variables"} to hide it.

Add a `when green flag clicked`{:class="block3events"} block to the Stage that sets both to `0`.

```blocks3
when green flag clicked
set [score v] to (0)
set [stuff to smash v] to (0)
```
