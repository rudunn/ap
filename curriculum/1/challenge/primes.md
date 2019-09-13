<code>
    
#include <stdio.h>
#include <cs50.h>

int main(void)
{
    bool is_prime;
    int counter = 1;
    int i = 3;
    int prime_numbers = 100;

    printf("%i, ", 2);
    //for (int i = 3; i < 100; i++)
    while (counter < prime_numbers)
    {
        is_prime = true;
        for (int j = 2; j < i; j++)
        {
            if (i % j == 0)
            {
                is_prime = false;
            }
        }
        if (is_prime)
        {
            printf("%i", i);

            counter++;
            if (counter < prime_numbers)
            {
                printf(", ");
            }
            else
            {
                printf("\n");
            }
        }
        i++;
    }
}

</code>
