# EX 1A Reverse a String
## DATE:26-4-25
## AIM:
To write a program to create a recursive function to reverse a string.

## Algorithm
1.Define a recursive function revstr that takes a string as input.

2.Check if the length of the string is zero (base case).

3.If true, return the string.

4.Otherwise, call revstr on the substring excluding the first character and concatenate the first character at the end.

5.Take input from the user and call the recursive function.

6.Print the result.

## Program:
```
/*
Program to implement Reverse a String
Developed by: S.keerthivasan
Register Number:  212222040076
*/

def rev(a):
    if len(a)==0:
        return a
    return rev(a[1:]) + a[0]
    
a=input()
print(rev(a))
```

## Output:

![1a](https://github.com/user-attachments/assets/e1cd87d8-360b-448c-bdbd-dc819fa86f24)


## Result:
The program successfully reverses the input string using recursion. When the user provides an input string, the output displays the reversed version of the string
