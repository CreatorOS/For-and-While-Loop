# for and while loop

Solidity supports `for`, `while`, and `do while` loops.

Don't write loops that are unbounded as this can hit the gas limit, causing your transaction to fail.

For the reason above, `while` and `do while` loops are rarely used.

## for loop

Let's start with a simple `for` loop.
It will run from 0 to 10.
But it will not run 10 times. If i is 5 then it will stop.
If i is 3 it will skip to 4 before checking the condition if i is 5.

```
    for (uint i = 0; i < 10; i++) {
        if (i == 3) {
            // Skip to next iteration with continue
            continue;
        }
        if (i == 5) {
            // Exit loop with break
            break;
        }
    }
```

## while loop

Let's write a `while` loop that will run until j is 10.
We will use `j++` to increment j inside the loop.

```
    uint j;
    while (j < 10) {
        j++;
    }
```
