[link](https://www.geeksforgeeks.org/find-the-largest-three-elements-in-an-array/)
Given an array with all distinct elements, find the largest three elements. Expected time complexity is O(n) and extra space is O(1). 

Examples :

Input: arr[] = {10, 4, 3, 50, 23, 90}
Output: 90, 50, 23
```python
def func(arr):
    max=arr[0]
    for i in range(len(arr)):
        if arr[i]>max:
            max=arr[i]
    return max
arr = [10, 4, 3, 50, 23, 90]
max1=func(arr)
k=[]
k.append(max1)
arr.remove(max1)
max2=func(arr)
arr.remove(max2)
max3=func(arr)
arr.remove(max3)

print(max1,max2,max3)
```
