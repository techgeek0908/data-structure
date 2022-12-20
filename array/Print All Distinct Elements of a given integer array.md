[link](https://www.geeksforgeeks.org/python-convert-number-to-list-of-integers/)
```
Print All Distinct Elements of a given integer array  
---
Example: Input: arr[] = {12, 10, 9, 45, 2, 10, 10, 45}  
Output: 12, 10, 9, 45, 2  
```
---
```python
def func(arr):
    res=[]
    for i in range(len(arr)):
        if arr[i] not in res:
            res.append(arr[i])
    return res 

arr=[12, 10, 9, 45, 2, 10, 10, 45]
output=func(arr)
print(output) 
```
