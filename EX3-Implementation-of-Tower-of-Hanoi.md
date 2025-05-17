# EX3 Implementation of Tower of Hanoi

## DATE:

## AIM:
To write a C program to implement Tower of Hanoi

## Algorithm
1. Start the program.
2. Check if n is greater than 0.
3. Recursively move n-1 disks from source (x) to auxiliary (z) using destination (y).
4. Print the move of the n-th disk from source (x) to destination (y).
5. Recursively move n-1 disks from auxiliary (z) to destination (y) using source (x).
6. The function is called initially with TOH(n, 'A', 'B', 'C') where 'A', 'B', and 'C' are the rods.
7. End
  

## Program:
```
/*
Program to implement Tower of Hanoi
Developed by: SADHANA SHREE B
RegisterNumber: 212223230177

#include<stdio.h>
void TOH(int n,char x,char y,char z)
{
  if(n>0){
      TOH(n-1,x,z,y);
      printf("%c to %c\n",x,y);
      TOH(n-1,z,y,x);
  }
}
int main()
{
    TOH(3,'A','B','C');
}
*/
```

## Output:
![Screenshot 2025-05-17 224717](https://github.com/user-attachments/assets/d738f8ed-73f7-40c1-a974-a20944490a1e)



## Result:
Thus, the C program to implement Tower of Hanoi using recursion is implemented successfully.
