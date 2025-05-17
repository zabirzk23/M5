# EX-21-POINTERS
# AIM:
Write a C program to convert a 23.65 into 25 using pointer

## ALGORITHM:
1.	Declare a double variable to hold the floating-point number (23.65).
2.	Declare a pointer to double to point to the address of the variable.
3.	Use the pointer to modify the value to 25.0.
4.	Print the modified value.

## PROGRAM:

```

#include <stdio.h>

int main() {
    double x = 23.65;
    double *p = &x;
    *p = 25.0;
    printf("%.1f", x);
    return 0;
}

```
## OUTPUT:
 	
![Screenshot 2025-05-17 161722](https://github.com/user-attachments/assets/9c983718-8bff-45ca-a7db-6134942dba2f)

## RESULT:
Thus the program to convert a 23.65 into 25 using pointer has been executed successfully.
 
 


# EX-22-FUNCTIONS AND STORAGE CLASS

## AIM:

Write a C program to calculate the Product of first 12 natural numbers using Recursion

## ALGORITHM:

1.	Define a recursive function calculateProduct that takes an integer parameter n.
2.	Return n multiplied by the result of the calculateProduct function called with n - 1.
3.	Declare an integer variable n and an unsigned long long variable product.
4.	Initialize n with the value 12 (for the first 12 natural numbers).
5.	Call the calculateProduct function with n and store the result in the product variable.
6.	Print the result, indicating it is the product of the first 12 natural numbers.

## PROGRAM:

```

#include <stdio.h>

unsigned long long f(int n) {
    if(n == 1) return 1;
    return n * f(n - 1);
}

int main() {
    int n = 12;
    unsigned long long p = f(n);
    printf("%llu", p);
    return 0;
}

```
## OUTPUT:

![Screenshot 2025-05-17 161949](https://github.com/user-attachments/assets/4b4c731e-d0dc-40a7-aea5-161609c93f3e)


## RESULT:

Thus the program has been executed successfully.
 
 


# EX-23-ARRAYS AND ITS OPERATIONS

## AIM:

Write C Program to find Sum of each row of a Matrix

## ALGORITHM:

1.	Declare and initialize the matrix with the desired values.
2.	Create a loop to iterate through each row of the matrix.
3.	Inside the loop, calculate the sum of the elements in each row.
4.	Print the sum for each row.

## PROGRAM:

```

#include <stdio.h>

int main() {
    int a[3][3] = {{1,2,3},{4,5,6},{7,8,9}};
    int i, j, s;
    for(i = 0; i < 3; i++) {
        s = 0;
        for(j = 0; j < 3; j++) {
            s += a[i][j];
        }
        printf("%d\n", s);
    }
    return 0;
}

```

## OUTPUT


 ![Screenshot 2025-05-17 162235](https://github.com/user-attachments/assets/57b90854-5d3a-443e-aeb0-e59753c06db2)

 

 ## RESULT
 
Thus the program has been executed successfully.

# EX-24-STRINGS

## AIM:

Write C program for the below pyramid string pattern. Enter a string: PROGRAM Enter number of rows: 5 P R O G R A M P R O G R A M P R O G R A M

## ALGORITHM:

1.	Input the number of rows for the pyramid (e.g., num_rows).
2.	Initialize variables:i for the row count (starting from 1),j for the character count (starting from 1)
3.	Start a loop for i from 1 to num_rows (for each row of the pyramid).
4.	Calculate the midpoint position as midpoint = (2 * num_rows - 1) / 2.
5.	End the program.

## PROGRAM:

```

#include <stdio.h>
#include <string.h>

int main() {
    char s[100];
    int r, i, j, k = 0;
    scanf("%s", s);
    scanf("%d", &r);
    for(i = 0; i < r; i++) {
        for(j = 0; j < r - i - 1; j++) printf(" ");
        for(j = 0; j <= i; j++) {
            printf("%c ", s[k]);
            k = (k + 1) % strlen(s);
        }
        printf("\n");
    }
    return 0;
}

```
 ## OUTPUT

 ![Screenshot 2025-05-17 162609](https://github.com/user-attachments/assets/5de78135-4f1b-4b82-b161-3c5dfed74196)

## RESULT

Thus the C program to String process executed successfully.



# EX -25 –DISPLAYING ARRAYS USING POINTERS
## AIM

Write a c program to read and display an array of any 6 integer elements using pointer

## ALGORITHM
Step 1: Start the program.
Step 2: Declare the following:
•	Integer variable i for iteration.
•	Integer variable n to store the number of elements.
•	Integer array arr[10] to hold up to 10 elements.
•	Integer pointer parr and initialize it to point to the array arr.
Step 3: Read the value of n (number of elements) from the user.
Step 4: Loop from i = 0 to i < n:
•	Read an integer value and store it in the address parr + i using pointer arithmetic.
Step 5: Loop from i = 0 to i < n:
•	Print the element at *(parr + i) using pointer dereferencing.
Step 6: End the program.

## PROGRAM

```

#include <stdio.h>

int main() {
    int a[10], *p = a, n, i;
    scanf("%d", &n);
    for(i = 0; i < n; i++) scanf("%d", p + i);
    for(i = 0; i < n; i++) printf("%d ", *(p + i));
    return 0;
}

```

## OUTPUT

 ![Screenshot 2025-05-17 162846](https://github.com/user-attachments/assets/37152603-e61b-4041-8089-efe41c9c5d1d)

## RESULT

Thus the C program to read and display an array of any 6 integer elements using pointer has been executed


