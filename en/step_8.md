## Smash with the space bar

Right now the signs vanish the moment Neil touches them. To make Neil *smash* them, the player should have to press the space bar too.

Change the `if then`{:class="block3control"} condition so it also checks whether the `space`{:class="block3sensing"} key is pressed, using an `and`{:class="block3operators"} block to join the two checks.

```blocks3
when I start as a clone
forever
+if <<touching (Neil v)?> and <key (space v) pressed?>> then
delete this clone
end
end
```

## Now run your code

Click the green flag. Neil now has to bump into a sign and press the space bar to smash it.
