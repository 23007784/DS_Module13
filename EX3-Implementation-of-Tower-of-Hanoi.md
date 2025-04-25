# EX3 Implementation of Tower of Hanoi
## DATE: 26.02.25
## AIM:
To write a C program to implement Tower of Hanoi

## Algorithm
1. Start the program.
2. Define the priority() function to return the priority of operators.
3. Initialize the string containing operators and operands.
4. Loop through each character in the string.
5. For each operator, call the priority() function to determine its priority.
6. Print the operator and its corresponding priority level.
7. End  

## Program:
```
/*
Program to implement Tower of Hanoi
Developed by: NIKSHITHA G
RegisterNumber:  212223110031
*/

#include<stdio.h>
void TOH(int n,char x,char y,char z)
{
  if ( n>0)
  {
      TOH(n-1,x,z,y);
      printf("%c to %c\n", x,y);
      TOH(n-1, z,y,x);
  }
  
}
int main()
{
    
    int n= 3;
    scanf("%d", &n);
    TOH(n ,'A', 'B' , 'C');
}
```

## Output:

![Screenshot 2025-04-25 131154](https://github.com/user-attachments/assets/8859e47b-8a2b-470b-b965-f7de53302595)


## Result:
Thus, the C program to implement Tower of Hanoi using recursion is implemented successfully.
