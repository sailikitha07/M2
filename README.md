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

![Screenshot 2025-04-29 171436](https://github.com/user-attachments/assets/0a7b9da7-0be1-475e-a6a9-5fa81d5ceaf1)









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
![Screenshot 2025-04-29 174913](https://github.com/user-attachments/assets/97e3ab5d-5c6a-4b6c-840f-d7dcd8f6fa57)





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
void add(int a, int b) {
    int sum = a + b;
    printf("Sum: %d + %d = %d\n", a, b, sum);
}
void subtract(int a, int b) {
    int diff = a - b;
    printf("Difference: %d - %d = %d\n", a, b, diff);
}
int main() {
    int num1, num2;
    printf("Enter first number: ");
    scanf("%d", &num1);
    printf("Enter second number: ");
    scanf("%d", &num2);
    add(num1, num2);
    subtract(num1, num2);
    return 0;
}
```
## OUTPUT:
![Screenshot 2025-04-29 175318](https://github.com/user-attachments/assets/6ff6e29c-06fa-4caa-b45a-aab299982bc6)


## RESULT:

Thus the program to perform addition and subtraction of two numbers using functions has been executed successfully
 
 


# EX-09-Use For Loop

## AIM:

Write a c program to find the sum of odd digits using for loop

## ALGORITHM:

1. Read an integer `n` from the user.
2. Initialize `sum` to 0.
3. Loop from 1 to `n`.
4. Check if each number is odd and add to `sum`.
5. Print the sum of odd numbers.
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

![Screenshot 2025-04-29 180138](https://github.com/user-attachments/assets/07a06c33-82aa-444a-b1fd-db75afd1573e)



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
![Screenshot 2025-04-29 180655](https://github.com/user-attachments/assets/4bde111e-2f38-439d-a49f-cda800c22829)

## RESULT:
The program correctly computes the factorial of a given number using a separate function and displays the result.
 
