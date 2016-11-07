# The Meanie Genie Puzzle

9 identical looking stones.  One weighs slightly more than the others, which are identical.

Given two balance scales that can only be used once, can we determine with certainty which is the heavier stone?

## Strategy:

1. take 3 away - weigh the other 6, do they balance?

2. yes - then the 3 contain the valuable stone. weigh any two of them.  If they balance, the other stone is it.  If they don't, you know which stone it is.

3. no - then the 6 contain the valuable stone and you know the 3 in which they fall (the heavier half).  Repeat step above - i.e. weigh any two stones.  If they balance, its the third stone.  If they don't, you have your stone.  

