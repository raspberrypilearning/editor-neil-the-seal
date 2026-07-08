## Fill the town with signs

Now give Neil something to smash.

You'll use clones to scatter stop signs around the town.

![sign sprite](images/sign-sprite.png)

## Step 1

Click on the `Sign`{:class="block3looks"} sprite.

Add a `when green flag clicked`{:class="block3events"} block and a `show`{:class="block3looks"} block, then use a `repeat ()`{:class="block3control"} loop to move to six random spots, making a clone at each one.

```blocks3
when green flag clicked
show
repeat (6)
go to x: (pick random (-220) to (220)) y: (pick random (-100) to (130))
create clone of (myself v)
end
```

## Step 2

The original sign is still on show.

Add a `hide`{:class="block3looks"} block to the end of the script, so only the six clones are left visible.

```blocks3
repeat (6)
go to x: (pick random (-220) to (220)) y: (pick random (-100) to (130))
create clone of (myself v)
end
+hide
```

## Now run your code

Click the green flag.

Six stop signs appear around the town.
