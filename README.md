# EX-06 - Looping
## AIM:
Write a C program to print even numbers ranging from M to N (including M and N values).

## ALGORITHM:
1.	Declare two integer variables to store the values of M and N.
2.	Use the printf function to prompt the user to enter the values of M and N.
3.	Use the scanf function to read the values of M and N from the user.
4.	Use a loop (for or while) to iterate from M to N.
5.	Inside the loop, check if the current number is even.
6.	If the current number is even, print it.
7.	Continue the loop until you have iterated through all numbers from M to N.

## PROGRAM:
```
#include <stdio.h>
int main() {
    int M, N;
    printf("Enter starting number (M): ");
    scanf("%d", &M);
    printf("Enter ending number (N): ");
    scanf("%d", &N);
    printf("Even numbers between %d and %d: ", M, N);
    for (int i = M; i <= N; i++) {
        if (i % 2 == 0) {
            printf("%d ", i);
        }
    }
    printf("\n");
    return 0;
}
```
## OUTPUT:
![Screenshot 2025-04-29 171436](https://github.com/user-attachments/assets/84bfd100-f51c-4b50-b6a1-3a82115d5ce4)










## RESULT:
Thus the program to print even numbers ranging from M to N (including M and N values) has been executed successfully
 
 


# EX-07-Nested-loop

## AIM:

Write a C program to print the given triangular pattern using loop.

## ALGORITHM:

1.	Declare a variable to store the number of rows in the triangle.
2.	Use the printf function to prompt the user to enter the number of rows.
3.	Use a loop (for or while) to iterate through each row.
4.	Inside the loop, use another loop to print the desired number of asterisks for each row.
5.	Continue the loop until you have printed the entire triangular pattern.

## PROGRAM:
```
#include <stdio.h>
int main() {
    int rows;
    printf("Enter number of rows: ");
    scanf("%d", &rows);

    for (int i = 1; i <= rows; i++) {
        for (int j = 1; j <= i; j++) {
            printf("%d ",j);
        }
        printf("\n");
    }

    return 0;
}
```
## OUTPUT:
![Screenshot 2025-04-29 174913](https://github.com/user-attachments/assets/d7d72517-9278-4a5d-82fa-2405c0d1b444)





## RESULT:

Thus the program to print the given triangular pattern using loop has been executed successfully
 
 


# EX-08-Functions

## AIM:

Write a C program to perform addition and subtraction of two numbers using functions (with argument and without return type).

## ALGORITHM:

1.	Declare two functions, one for addition and one for subtraction. Both functions should take two integer arguments.
2.	Inside the addition & subtraction function, add & subtract the two numbers and print the result.
3.	In the main function, declare two integer variables and read their values from the user.
4.	Call the addition and subtraction functions, passing the two numbers as arguments.

## PROGRAM:
```
#include <stdio.h>
void addition(int a, int b) {
    int sum = a + b;
    printf("Sum: %d + %d = %d\n", a, b, sum);
}
void subtraction(int a, int b) {
    int diff = a - b;
    printf("Difference: %d - %d = %d\n", a, b, diff);
}
int main() {
    int num1, num2;
    printf("Enter first number: ");
    scanf("%d", &num1);
    printf("Enter second number: ");
    scanf("%d", &num2);
    addition(num1, num2);
    subtraction(num1, num2);
    return 0;
}
```
## OUTPUT:
![Screenshot 2025-04-29 175318](https://github.com/user-attachments/assets/7327513e-5daa-419d-b2e8-4dd2f8d344fa)






## RESULT:

Thus the program to perform addition and subtraction of two numbers using functions has been executed successfully
 
 


# EX-09-Use For Loop

## AIM:

Write a c program to find the sum of odd digits using for loop

## ALGORITHM:

1.	Declare variables to store the input number and the sum of odd digits.
2.	Initialize the sum of odd digits to 0.
3.	Use a for loop to iterate through each digit of the input number.
4.	Inside the loop, extract the rightmost digit of the number (using the modulo operator % and division by 10).
5.	If the digit is odd, add it to the sum of odd digits.
6.	Print the sum of odd digits.

## PROGRAM:
```
#include <stdio.h>
int main() {
    int n, sum = 0;
    printf("Enter the number:");
    scanf("%d", &n);
    for (int i = 1; i <= n; i++) {
        if (i % 2 != 0) sum += i;
    }
    printf("Sum of odd numbers from %d to %d is %d",1,n,sum);
    return 0;
}
```
## OUTPUT:

![Screenshot 2025-04-29 180138](https://github.com/user-attachments/assets/f6d3c22a-a7d0-43a2-b650-05f839f6396d)



## RESULT:

Thus the program to find the sum of odd digits using for loop has been executed successfully.




# EX – 10 - Factorial of a Number Using a Function
## AIM:
To write a C program that calculates the factorial of a given number using a user-defined function.
## ALGORITHM:
1.	Start
2.	Declare the function fact().
3.	In the main() function, call the fact() function.
4.	In fact() function:
a.	Declare variables i, N, and fact (initialized to 1).
b.	Read an integer N from the user.
c.	Use a for loop from 1 to N:
i.	Multiply fact by i in each iteration.
d.	After the loop, print the factorial value.
5.	End

## PROGRAM:
```
#include <stdio.h>
int fact(int x)
{
    int i,fac=1;
    for(i=1 ; i<=x ; i++)
    {
        fac*=i;
    }
    return fac;
}
int main()
{
    int n;
    scanf("%d",&n);
    int f=fact(n);
    printf("Factorial value is: %d",f);
    return 0;
}
```

## OUTPUT:
![Screenshot 2025-04-29 180655](https://github.com/user-attachments/assets/d31c2ba5-67d6-4a00-bfbb-fdd4e6080e2e)

## RESULT:
The program correctly computes the factorial of a given number using a separate function and displays the result.
 
