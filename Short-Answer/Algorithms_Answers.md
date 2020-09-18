#### Please add your answers to the ***Analysis of  Algorithms*** exercises here.

## Exercise I
## Analyzing runtime (3 points) - identify runtime and justify answer
a) Runtime is O(n) because runtime grows linearly with the size of the input.

n = 2
a = 0

while (a < n * n * n): 
      a = a + n * n 

runs: 2
while (0 < 8): 
      a = 4
while (4 < 8): 
      a = 8

b) Runtime is O(n2) because runtime grows exponentially with the size of the input (nested loop).


c) Runtime is O(n) because there will be one operation per recursive call.


## Exercise II
## Find the highest floor (3 points)
## Suppose that you have an n-story building and plenty of eggs. Suppose also that an egg gets broken if it is thrown off floor f or higher, and doesn't get broken if dropped off a floor less than floor f. Devise a strategy to determine the value of f such that the number of dropped + broken eggs is minimized.
## Write out your proposed algorithm in plain English or pseudocode AND give the runtime complexity of your solution.

Binary Search O(log n) because it's halving # of levels

- set pointers 
      - start = 0 
      - end = # of levels
- loop that will continue while the start pointer is less than or equal to the end pointer
- find middle and test if it breaks 
      - if egg breaks, move down a level (set end to middle - 1) and test again
      - otherwise, move up (set start to middle + 1) and test again
      - otherwise return middle 


