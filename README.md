# DBNC-INC
Function quizz
#include <stdio.h>
int main() 
{
    int N, M;                                                         // integer declaration for two dimensions M & N 
    printf("Enter the dimensions of the rectangular paper (N x M): ");// User prompt for screen printing 
    scanf("%d %d", &N, &M);                                           // User prompt for getting  values 
    printf("Series of squares:\n");     
    while (N > 0 && M > 0)                                             //conditional statement for N and M 
    {  
        if (N >= M)                                                    // if N is greater than or equal to M
        {
            printf("%d x %d\n", M, M);                                // print  as M x M 
            N -= M;                                                   // and subratcs M from N 
        } 
        else                                                          // otherwise print as N xN
        { 
            printf("%d x %d\n", N, N);
            M -= N;                                                  // and subratcs N from M 
        }
    }
    if (N == 1 && M == 1) 
    { 
        printf("1 x 1\n");                                           // This will print if Both dimension are 1 (unity )
    }
    return 0;
}
