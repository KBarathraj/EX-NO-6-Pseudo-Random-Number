# EX-NO-6-Pseudo-Random-Number

# AIM: 
Implementation of Pseudorandom Number Generation Using Standard library

# ALGORITHM:
Start the program and import the required libraries.
Seed the random number generator using the current time(i.e) rand(time(0));
Get the number of randon number to generate.
Pass the value for number of iterations and print the numbers.
End the program.

# PROGRAM:
```C
#include <stdio.h>
#include <stdlib.h>
#include <time.h>
//Program developed by BARATHRAJ K (212224230033)
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
# OUTPUT:
<img width="2385" height="1213" alt="image" src="https://github.com/user-attachments/assets/5e918262-fd1b-4d1d-a32c-41024d625e70" />

# RESULT:
Thus, we have successfully implemented pseudo-random number generation using the standard library in C.
