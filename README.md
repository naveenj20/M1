### NAME : Naveen Jaisanker
### REG. NO. : 212224110039

# EX-01-Datatypes-Operators

## AIM:
Write a C program to read 3 characters one by one and print the characters in a reverse order.

## ALGORITHM:
1.	Declare three character variables to store the input characters.
2.	Use the scanf function to read the characters one by one from the user.
3.	Print the characters in reverse order using the printf function.
4.	End the program.

## PROGRAM:

```
#include <stdio.h>
int main() {
    char ch1, ch2, ch3;
    printf("Enter three characters one by one:\n");
    printf("First: ");
    scanf(" %c", &ch1);
    printf("Second: ");
    scanf(" %c", &ch2);
    printf("Third: ");
    scanf(" %c", &ch3);
    printf("\nYou entered (in reverse order): %c %c %c\n", ch3, ch2, ch1);
    return 0;
}
```

## OUTPUT:

![Screenshot 2025-04-28 084142](https://github.com/user-attachments/assets/23597cd6-1f4a-4947-8d2c-50883045cc9a)

## RESULT:
Thus the program to read 3 characters one by one and print the characters in a reverse order has been executed successfully.


# EX-02- Conditional-Statements

## AIM:
Write a C program to read A values and check whether A is positive number or not.

# ALGORITHM:
1.	Declare a variable to store the input value A.
2.	Use the scanf function to read the value of A from the user.
3.	Check if the value of A is greater than zero.
4.	If A is greater than zero, print a message indicating that it's a positive number. 
5.	Otherwise, print a message indicating that it's not a positive number.
6.End the program.

# PROGRAM:

```
#include <stdio.h>
int main() {
    int A;
    printf("Please enter an integer value: ");
    scanf("%d", &A);
    if (A > 0) {
        printf("%d is positive.\n", A);
    } else if (A < 0) {
        printf("%d is negative.\n", A);
    } else {
        printf("The number is zero.\n");
    }
    return 0;
}
```

# OUTPUT:

![Screenshot 2025-04-28 084326](https://github.com/user-attachments/assets/8d228363-4bb3-4ea2-89d7-e950f38ab4be)

![Screenshot 2025-04-28 084336](https://github.com/user-attachments/assets/d2679b72-9f1e-470e-bf92-35af6ebe37d5)

![Screenshot 2025-04-28 084345](https://github.com/user-attachments/assets/4d5e6da4-a4e9-4a44-a16e-9d53af9c2435)

# RESULT:
Thus the program to read A values and check whether A is positive number or not has been executed successfully.


# EX-03- Operators-Expressions

## AIM:
Write a program to find minimum between two fraction numbers using conditional operator or ternary operator.

## ALGORITHM:
1.	Declare variables to store the two fraction numbers and the result.
2.	Use the printf function to prompt the user to enter the first fraction number (numerator and denominator separately).
3.	Use the scanf function to read the numerator and denominator of the first fraction.
4.	Repeat steps 2 and 3 to get the second fraction from the user.
5.	Calculate the decimal values of both fractions by dividing the numerators by the denominators.
6.	Use the conditional (ternary) operator to compare the decimal values and store the minimum value in the result variable.
7.	Print the minimum value.

## PROGRAM:

```
#include <stdio.h>
int main() {
    int num1, den1, num2, den2;
    float frac1, frac2, min;
    printf("Enter numerator and denominator of the first fraction: ");
    scanf("%d%d", &num1, &den1);
    printf("Enter numerator and denominator of the second fraction: ");
    scanf("%d%d", &num2, &den2);
    if (den1 == 0 || den2 == 0) {
        printf("Denominator cannot be zero.\n");
        return 1;
    }
    frac1 = (float)num1 / den1;
    frac2 = (float)num2 / den2;
    min = (frac1 < frac2) ? frac1 : frac2;
    printf("The smaller fraction value is: %.2f\n", min);
    return 0;
}
```

## OUTPUT:

![Screenshot 2025-04-28 084520](https://github.com/user-attachments/assets/a8915695-fb24-439d-96a1-86c526dbdeea)

## RESULT:
Thus the program to find minimum between two fraction numbers using conditional operator or ternary operator has been executed successfully.



# EX-04- Using Conditional Statements

## AIM:
Write a C program to check whether the input value is equal to 1 using simple if statement

## ALGORITHM:
1.	Declare a variable to store the input value.
2.	Use the scanf function to read the input value from the user.
3.	Use an if statement to check if the input value is equal to 1.
4.	If the condition in the if statement is true, print a message indicating that the input value is equal to 1.
5.	Otherwise, print a message indicating that it's not equal to 1.
6.	End the program.

## PROGRAM:

```
#include <stdio.h>
int main() {
    int value;
    printf("Please enter an integer: ");
    scanf("%d", &value);
    if (value == 1) {
        printf("You entered 1.\n");
    } else {
        printf("You did not enter 1.\n");
    }
    return 0;
}
```

## OUTPUT:

![Screenshot 2025-04-28 084641](https://github.com/user-attachments/assets/44ed2b37-2a63-4964-8e3f-6be06328a19f)

![Screenshot 2025-04-28 084650](https://github.com/user-attachments/assets/e06fdb24-c163-4c04-9a2a-d46892eb038f)


## RESULT:
Thus the program to check whether the input value is equal to 1 using simple if statement has been executed successfully


# EX-05- Calculating Total, Percentage, And Division Using Conditional Statements 

## AIM:
To write a C program that reads marks of three subjects, calculates the total and percentage, and then determines the division (First, Second, Pass, or Fail) based on the percentage and minimum marks criteria.

## ALGORITHM:
1.	Start
2.	Declare integer variables m1, m2, m3 for marks, and float variables tot, per.
3.	Input the marks for three subjects.
4.	Calculate total marks: tot = m1 + m2 + m3
5.	Calculate percentage: per = tot / 3
6.	Display total and percentage.
7.	Check if all marks are greater than or equal to 40:
8.	If yes:
a.	If percentage >= 60: Print “Division = First”
b.	Else if percentage >= 48: Print “Division = Second”
c.	Else if percentage >= 36: Print “Division = Pass”
9.	Else: Print “Division = Fail”
10.	End
    
## PROGRAM:

```
#include <stdio.h>
int main() {
    int m1, m2, m3;
    float tot, per;
    printf("Enter marks for three subjects: ");
    scanf("%d%d%d", &m1, &m2, &m3);
    tot = m1 + m2 + m3;
    per = tot / 3.0; 
    printf("\nTotal Marks = %.2f\n", tot);
    printf("Percentage = %.2f%%\n", per);
    if (m1 >= 40 && m2 >= 40 && m3 >= 40) {
        if (per >= 60) {
            printf("Division = First\n");
        } else if (per >= 48) {
            printf("Division = Second\n");
        } else if (per >= 36) {
            printf("Division = Pass\n");
        } else {
            printf("Division = Fail\n");
        }
    } else {
        printf("Division = Fail\n");
    }
    return 0;
}
```

## OUTPUT:

![Screenshot 2025-04-28 084825](https://github.com/user-attachments/assets/55c72b39-efa0-4805-b205-f9c7c5e4fae0)

![Screenshot 2025-04-28 084836](https://github.com/user-attachments/assets/7bdbd409-6486-4767-a67a-297ed90f761d)

## RESULT:
The program successfully takes three subject marks, calculates the total and percentage, and correctly determines the division based on predefined grading logic.

