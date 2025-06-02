# EX1(C) Implementation of Tower of Hanoi
## DATE: 26.02.25
## AIM:
To write a C program to implement Tower of Hanoi

## Algorithm
1. Define the recursive function with parameters for number of disks and source, auxiliary, and destination rods.

2. Check the base case – if only one disk, move it directly from source to destination.

3. Recursively move (n-1) disks from source to auxiliary using destinaation as temporary storage.

4. Move the remaining disk from source to destination.

5. Recursively move (n-1) disks from auxiliary to destination using source as temporary storage.

## Program:
```
/*
Program to implement Tower of Hanoi
Developed by:Jidhesh P
RegisterNumber: 212223040078
*/
```
```
#include<stdio.h>
void TOH(int n,char x,char y,char z)
{
    if(n>0)
    {
       TOH(n-1,x,z,y);
       printf("%c to %c\n",x,y);
       TOH(n-1,z,y,x);
    }
}
int main()
{
   int n=3;
   char x;
   char y;
   char z;
   x='A';
   y='B';
   z='C';
   TOH(n,x,y,z); 
}
```
## Output:
![image](https://github.com/user-attachments/assets/0b23ee51-be1e-4e27-a601-12dc381da124)



## Result:
Thus, the C program to implement Tower of Hanoi using recursion is implemented successfully.
