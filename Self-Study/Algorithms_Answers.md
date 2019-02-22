a) a = 0
while (a < n _ n _ n):
a = a + n \* n

O(n) it grows by n. So if n = 2 then there are two runs of the while loop. If n= 3, there are 3 runs of the while loop, and so on.

b) b) sum = 0

    for i in range(n):
      i += 1
      for j in range(i + 1, n):
        j += 1
        for k in range(j + 1, n):
          k += 1
          for l in range(k + 1, 10 + k):
            l += 1
            sum += 1

O(n^2) loops j and k run less than the i loop. However, as n gets larger K running more than N. the graph grows similar to O(n^2). As the larger the number the more K runs exponentially.

c) def bunnieEars(bunnies):
if bunnies == 0:
return 0

      return 2 + bunnyEars(bunnies-1)

the program would not run, because bunnyEars is not a recursive call of the bunnieEars function. If this is a type-o than it would be O(n) as the number of operations increase by n.

Exercise II

Suppose that you have an n-story building and plenty of eggs. Suppose also that an egg gets broken if it is thrown off floor f or higher, and doesn't get broken if dropped off a floor less than floor f. Devise a strategy to determine the value of f such that the number of dropped eggs is minimized.

Write out your proposed algorithm in plain English or pseudocode and give the runtime complexity of your solution.

1. so the best way to do this is a binary search.

2. Find the middle of the building and drop an egg

3. if the egg does not break go to step 4, else step 5

4. Go up, higher in the building. Split the amount of floors left in half. See if the egg break.
   Move accordingly from there in the same fashion cutting the remianing floors in half.

5. Go lower, split num of floors below in haf and continue the process until you find the highest floor that does not break the egg.

binary search has a time complexity of Θ(log(n)).
