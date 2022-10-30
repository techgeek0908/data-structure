[link](https://www.geeksforgeeks.org/array-rotation/)

Given an array of integers arr[] of size N and an integer, the task is to rotate the array elements to the left by d positions.

Examples:  

Input: 
arr[] = {1, 2, 3, 4, 5, 6, 7}, d = 2
Output: 3 4 5 6 7 1 2

Input: arr[] = {3, 4, 5, 6, 7, 1, 2}, d=2
Output: 5 6 7 1 2 3 4

---
```python
def func(arr, d):
    k = arr.index(d)
    newList = []
    newList = arr[k+1:]+arr[0:k+1]
    return newList
 
arr = [1, 2, 3, 4, 5, 6, 7]
d = 2

arr = func(arr, d)
for i in arr:
    print(i, end=" ")
```
