# EX 1 Display operator precedence in the infix expression.
## DATE: 21/02/2025
## AIM:
To write a C program to find and display the priority of the operator in the given Postfix expression

## Algorithm
1. Start the program.
2. Define the priority() function to return the priority of operators.
3. Initialize the string containing operators and operands.
4. Loop through each character in the string.
5. For each operator, call the priority() function to determine its priority.
6. Print the operator and its corresponding priority level.
7. End.  

## Program:
```
/*
Program to find and display the priority of the operator in the given Postfix expression
Developed by: SADHANA SHREE B
RegisterNumber: 212223230177

#include <stdio.h>
#include<string.h>

 int priorityg(char x)
{
    if(x == '&' || x == '|')
        return 1;
    else if(x=='+' || x=='-')
        return 2;
    else if(x=='*' || x=='/')
        return 4;
    else
        return -1;
}

int main()
{
   int i,j;
   char ch[100]= "100 200 + 2 / 5 * 7 |";
   for (i = 0; ch[i] != '\0'; i++) {
        if (ch[i] == '+' || ch[i] == '-' || ch[i] == '*' || ch[i] == '/' || ch[i] == '&' || ch[i] == '|') {
            j=priorityg(ch[i]);
            switch(j)
           {
               case 1:
               printf("%c  ----> Lowest Priority\n",ch[i]);
               break;
               case 2:
               printf("%c  ----> Second Lowest Priority\n",ch[i]);
               break;
               case 4:
               printf("%c  ----> Second Highest Priority\n",ch[i]);
               break;
               default:
               printf("Invalid\n");
           }
        }
   
    
    }return 0;
   
}
*/
```

## Output:
![Screenshot 2025-05-17 225314](https://github.com/user-attachments/assets/00670a3e-aad2-444a-8256-b1e3ffe2d964)


## Result:
Thus the C program to find and display the priority of the operator in the given Postfix expression is implemented successfully
