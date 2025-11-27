
QUICKSORT(A, low, high):
1. if low < high then
2.      p = PARTITION(A, low, high)
3.      QUICKSORT(A, low, p-1)
4.      QUICKSORT(A, p+1, high)

PARTITION(A, low, high):
1. pivot = A[high]
2. i = low - 1
3. for j = low to high-1 do
4.      if A[j] <= pivot then
5.          i = i + 1
6.          swap A[i] and A[j]
7. swap A[i+1] and A[high]
8. return i+1
