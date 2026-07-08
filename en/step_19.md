## Neil reacts to being caught

Now Neil needs to react when he's caught.

![neil sprite](images/neil-sprite.png)

Click on the `Neil`{:class="block3looks"} sprite.

Add a `when I receive ()`{:class="block3events"} block for the `got ya` message.

Send Neil back to his starting position, then make him `say () for () seconds`{:class="block3looks"} to say "Hey!".

```blocks3
when I receive (got ya v)
go to x: (0) y: (-40)
say [Hey!] for (0.6) seconds
```

## Now run your code

Click the green flag and let the Ranger catch Neil.

Neil says "Hey!", pops back to the start, and loses a life.
