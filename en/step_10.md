## Count and score the signs

Click on the `Sign`{:class="block3looks"} sprite.

![sign sprite](images/sign-sprite.png)

## Step 1

Inside the `repeat ()`{:class="block3control"} loop, add a `change stuff to smash by ()`{:class="block3variables"} block to count each clone. Then add a `wait () seconds`{:class="block3control"} block for `0.1` seconds at the very top of the script.

```blocks3
when green flag clicked
+wait (0.1) seconds
show
repeat (6)
go to x: (pick random (-220) to (220)) y: (pick random (-100) to (130))
create clone of (myself v)
+change [stuff to smash v] by (1)
end
hide
```

## Tip

Both this script and the Stage's setup script start when the green flag is clicked, so they run at the same time. Without the short wait, the signs could start counting before the Stage sets `stuff to smash` back to `0`, and the total would come out wrong.

## Step 2

In the clone script, inside the `if then`{:class="block3control"} block, add a `change score by ()`{:class="block3variables"} block to add `10` points and a `change stuff to smash by ()`{:class="block3variables"} block to take away `1`.

```blocks3
when I start as a clone
forever
if <<touching (Neil v)?> and <key (space v) pressed?>> then
+change [score v] by (10)
+change [stuff to smash v] by (-1)
delete this clone
end
end
```

## Now run your code

Click the green flag and smash some signs. Your score goes up, and the amount of stuff left to smash goes down.
