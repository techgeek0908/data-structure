[link](https://www.geeksforgeeks.org/array-data-structure/#rearrange)

Given an array (or string), the task is to reverse the array/string.
Examples : 
 

Input  : arr[] = {1, 2, 3}
Output : arr[] = {3, 2, 1}

Input :  arr[] = {4, 5, 1, 2}
Output : arr[] = {2, 1, 5, 4}

```python
a=[4,2,6,4,8]
print(a[::-1])
```
---
```python
def reverse(alist):
    newList=[]
    for i in range(len(alist)-1,-1,-1):
        newList.append(alist[i])
    return newList

l=[1,2,3,4,5,6,7,8]
output=reverse(l)
print(output)
```
