# EX 1C Quick Sort
## DATE:26-5-25
## AIM:
To write a python program to implement quick sort using tha last element as pivot on the list of float values.

## Algorithm
1. Read n and take n floating-point inputs into an array arr.
2.Define a partition function to place the pivot in its correct position.
3.Define a recursive quickSort function using the partition logic.
4.Call quickSort(arr, 0, n - 1) to sort the entire array.
5.Print the sorted elements of arr.

## Program:
```
/*
Program to implement implement quick sort using the last element as pivot on the list of float values.
Developed by: S.keerthivasan
Register Number:  212222040076
*/
```
```
def partition(arr, low, high):
    pivot = arr[high]
    i = low - 1
    for j in range(low, high):
        if arr[j] <= pivot:
            i += 1
            arr[i], arr[j] = arr[j], arr[i]
    arr[i + 1], arr[high] = arr[high], arr[i + 1]
    return i + 1

def quickSort(arr, low, high):
    if low < high:
        pi = partition(arr, low, high)
        quickSort(arr, low, pi - 1)
        quickSort(arr, pi + 1, high)

n = int(input())
arr = [float(input()) for _ in range(n)]
print("Sorted array is:")
quickSort(arr,0,n-1)
for num in arr:
    print(num)
```

## Output:

![3](https://github.com/user-attachments/assets/7044f18f-fb4c-4772-90d5-c02572c1116a)


## Result:
The program successfully sorts the input array using the QuickSort algorithm, arranging the elements in ascending order.
