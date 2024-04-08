# Linear Search and Binary search
## Aim:
To write a program to perform linear search and binary search using python programming.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
## Linear Search:
1.	Start from the leftmost element of array[] and compare k with each element of array[] one by one.
2.	If k matches with an element in array[] , return the index.
3.	If k doesn’t match with any of elements in array[], return -1 or element not found.
## Binary Search:
1.	Set two pointers low and high at the lowest and the highest positions respectively.
2.	Find the middle element mid of the array ie. arr[(low + high)/2]
3.	If x == mid, then return mid.Else, compare the element to be searched with m.
4.	If x > mid, compare x with the middle element of the elements on the right side of mid. This is done by setting low to low = mid + 1.
5.	Else, compare x with the middle element of the elements on the left side of mid. This is done by setting high to high = mid - 1.
6.	Repeat steps 2 to 5 until low meets high
## Program:
i)	#Use a linear search method to match the item in a list.
```
''' 
Program to the maximum marks without using builtin functions.
Developed by: KEERTHIVASAN M
RegisterNumber: 212223100021
'''
def linearSearch(array,n,k):
    for i in range(n):
        if array[i]==k:
            return i
    return -1
array = eval(input())
array.sort()
k = eval(input()) 
n=len(array)
print(array)
result = linearSearch(array,n,k)
if result==-1:
    print("Element not found")
else:
    print("Element found at index: ",result) 


```
ii)	# Find the element in a list using Binary Search(Iterative Method).
```
''' 
Program to the maximum marks without using builtin functions.
Developed by: KEERTHIVASAN M
RegisterNumber: 212223100021
'''
def binarySearchIter(array, k, low, high):
    while low<=high:
        mid=low+(high-low)//2
        if array[mid]==k:
            return mid
        elif array[mid]<k:
            low=mid+1
        else:
            high=mid-1
    return -1
array = eval(input())
array.sort()
k = eval(input()) 
print(array)
res=binarySearchIter(array,k,0,len(array)-1)
if res==-1:
    print("Element not found")
else:
    print("Element found at index: ",res)




```
iii)	# Find the element in a list using Binary Search (recursive Method).
```
''' 
Program to the maximum marks without using builtin functions.
Developed by: KEERTHIVASAN M
RegisterNumber: 212223100021
'''
def binarySearchIter(array, k, low, high):
    while low<=high:
        mid=low+(high-low)//2
        if array[mid]==k:
            return mid
        elif array[mid]<k:
            low=mid+1
        else:
            high=mid-1
    return -1
array = eval(input())
array.sort()
k = eval(input()) 
print(array)
res=binarySearchIter(array,k,0,len(array)-1)
if res==-1:
    print("Element not found")
else:
    print("Element found at index: ",res)



```
## Sample Input and Output

![Screenshot 2024-03-24 193835](https://github.com/rdxkeerthi/Search-Algorithms/assets/147473120/f9dfc375-33f5-4b9d-931c-253686cb4a7d)

![Screenshot 2024-03-24 193821](https://github.com/rdxkeerthi/Search-Algorithms/assets/147473120/9aff4c60-ce15-49dd-95aa-e12d32cbffd6)

![Screenshot 2024-03-24 193805](https://github.com/rdxkeerthi/Search-Algorithms/assets/147473120/6a2407a0-d294-4a8f-afa9-7bacc65f7f1a)



## Result
Thus the linear search and binary search algorithm is implemented using python programming.
