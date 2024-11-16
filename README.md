# EX-NO-6-Pseudo-Random-Number

# AIM: 

Implementation of Pseudorandom Number Generation Using Standard library

# ALGORITHM
# Step 1:
Declare the necessary variables for storing the count of random numbers, minimum and maximum values, and the generated random number.

# Step 2:
Prompt the user for the number of random numbers to be generated (count), and ensure the input is a valid positive integer.

# Step 3:
Prompt the user to input the minimum (min) and maximum (max) values for the range. Validate that the maximum value is greater than the minimum.

# Step 4:
Use the srand(time(NULL)) function to seed the random number generator based on the current time.

# Step 5:
For the specified count, generate random numbers using the formula:

random_number=(rand()%(max−min+1))+min

Print each generated random number.
# PROGRAM
```
NAME: NIKSHITHA G
REG NO: 212223110031

#include <stdio.h>
#include <stdlib.h>
#include <time.h>

int main() 
{
    int count, min, max;
    printf("Enter the number of random numbers to generate: ");
    scanf("%d", &count);
    printf("Enter the minimum value: ");
    
    scanf("%d", &min);
    printf("Enter the maximum value: ");
    scanf("%d", &max);
    srand(time(NULL));
    printf("Pseudorandom numbers:\n");   
    for (int i = 0; i < count; i++) 
    {
        int random_number = (rand() % (max - min + 1)) + min;
        printf("%d ", random_number);
    }
    return 0;
}
```

# OUTPUT
![Screenshot (65)](https://github.com/user-attachments/assets/00e82ee2-1bdc-4801-8322-f2925b5524a2)



# RESULT
   Thus the Implementation of Pseudorandom Number Generation Using Standard library was executed successfully.
