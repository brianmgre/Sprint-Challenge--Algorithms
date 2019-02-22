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
