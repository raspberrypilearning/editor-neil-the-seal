## Add cars and barriers

Now add cars and barriers for Neil to smash too. Instead of coding them from scratch, you'll reuse the code you wrote for the stop signs.

## Step 1

Click on the `Sign`{:class="block3looks"} sprite. Drag each of its two scripts onto the `Car`{:class="block3looks"} sprite in the sprite list, then onto the `Barrier`{:class="block3looks"} sprite, to copy the code across. Both sprites already point their blocks at the right things, so the code works straight away.

--- no-print ---

![Animated image showing a script being dragged onto another sprite in the sprite list to copy it](images/copy-script.gif)

--- /no-print ---

## Step 2

Click on the `Car`{:class="block3looks"} sprite. In the `repeat ()`{:class="block3control"} loop, change the number to decide how many cars appear. Then do the same on the `Barrier`{:class="block3looks"} sprite.

## Step 3

Decide how many points each one is worth. On both the `Car`{:class="block3looks"} and `Barrier`{:class="block3looks"} sprites, change the number in the `change score by ()`{:class="block3variables"} block. Maybe some things are trickier to reach and should be worth more?

## Step 4

Choose where each type of object appears. In the `go to x: () y: ()`{:class="block3motion"} block, change the `pick random () to ()`{:class="block3operators"} numbers to set the area they spawn in — for example, keeping the cars low down so they stay on the road.

## Now run your code

Click the green flag. The town is now full of signs, cars, and barriers to smash — each worth the points you chose, in the places you picked.
