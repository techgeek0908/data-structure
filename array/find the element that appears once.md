[link](https://www.geeksforgeeks.org/find-element-appears-array-every-element-appears-twice/)

Given an array of integers. All numbers occur twice except one number which occurs once. Find the number in O(n) time & constant extra space.

Example : 

Input:  arr[] = {2, 3, 5, 4, 5, 3, 4}
Output: 2 

```python
def func(arr):
    res=[]
    for i in range (len(arr)):
        check=arr[i]
        count=0
        for j in range (len(arr)):
            if arr[j]==check:
                count+=1
        if count == 1:
            res.append(check)
    return res

arr=[2, 3, 5, 4, 5, 6, 3, 4]
output=func(arr)
print(output)
```
