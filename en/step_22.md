## The Ranger says goodbye

Make the Ranger respond when the game is over.

![ranger sprite](images/ranger-sprite.png)

Click on the `Ranger`{:class="block3looks"} sprite.

Add a `when I receive ()`{:class="block3events"} block for the `game over` message, and make the Ranger `say () for () seconds`{:class="block3looks"} to say "Off you go!".

```blocks3
when I receive (game over v)
say [Off you go!] for (1) seconds
```

You won't see this on its own yet — you'll test it after the next step.
