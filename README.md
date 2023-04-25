# SWAP-USING-POINTERS
In programming language, swapping of two numbers in c indicates swapping the values of two variables. Consider that you have the variables var1 and var2. Var1 has a value of 20 and Var2 has a value of 40. Therefore, after swapping, the values of var1 and var2 will be 40 and 20, respectively. 
Different Methods to Swap Two Numbers in C:
Swapping Two Numbers Using Third Variable
Swapping Two Numbers Using Without Using Third Variable
Swapping Function in C
Swap two numbers using pointers in C
rs

Lets write a C program to swap 2 numbers using pointers and function.

When we call the function, we pass the reference or address of the variable, so this method is called “Call by Reference“.

JAVA Program for SWAPPING of TWO Nu...

Pause

Unmute
Remaining Time -5:49


Fullscreen
JAVA Program for SWAPPING of TWO Numbers Using a Third Variable
Related Read:
Swap 2 Numbers Using a Temporary Variable: C
Function / Methods In C Programming Language
Basics of Pointers In C Programming Language

Video Tutorial: C Program To Swap Two Numbers using Pointers




YouTube Link: https://www.youtube.com/watch?v=snxBqbRYrhs [Watch the Video In Full Screen.]


Source Code: C Program To Swap Two Numbers using Pointers and Function
view plaincopy to clipboardprint?
#include<stdio.h>  
  
void swap(int*, int*);  
  
int main()  
{  
    int a, b;  
  
    printf("Enter values for a and b\n");  
    scanf("%d%d", &a, &b);  
  
    printf("\n\nBefore swapping: a = %d and b = %d\n", a, b);  
  
    swap(&a, &b);  
  
    printf("\nAfter swapping: a = %d and b = %d\n", a, b);  
  
    return 0;  
}  
  
void swap(int *x, int *y)  
{  
    int temp;  
  
    temp = *x;  
    *x   = *y;  
    *y   = temp;  
}  
Output 1:
Enter values for a and b
100
200

Before swapping: a = 100 and b = 200

After swapping: a = 200 and b = 100

Output 2:
Enter values for a and b
30
20

Before swapping: a = 30 and b = 20


After swapping: a = 20 and b = 30


Logic To Swap Two Numbers using Pointers and Function
We ask the user to enter values for variable a and b. We pass the address of variable a and b to function swap().

Inside function swap() we take a local variable temp. Since address of variable a and b are passed to swap() method, we take 2 pointer variables *x and *y. Pointer variable x holds the address of a and pointer variable y holds the address of b. Using below logic we swap the values present at address a( or x ) and b( or y ).


temp = *x;
*x = *y;
*y = temp;
