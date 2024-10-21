# EX-NO-6-Pseudo-Random-Number

# AIM: 

Implementation of Pseudorandom Number Generation Using Standard library

# Algorithm:
```
1.Algorithm for Pseudorandom Number Generation:

2.Accept user input for the number of random numbers (count), minimum value (min), and maximum value (max).

3.Initialize the random seed using the current time (srand(time(NULL))).

4.Start a loop that runs count times to generate random numbers.

5.In each iteration, calculate a random number between min and max using the formula (rand() % (max - min + 1)) + min

6.Print the generated random number.

7.Repeat until count random numbers are generated, then terminate the program.
```
# Program:
```

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
        printf("%d\n", random_number);
    }
    return 0;
}

```

# Output :

![Uploading image.png…]()


# Result:
Thus the program to generate random numbers is implemented successfully









