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



2. ---------->Question 
 Q2) Below is a link to a spreadsheet with two columns A and B such that:
A is the input
B is the output
Based on the spreadsheet, there exist a function such as  f that relates A to B which is:
Bi = f(Ai)
Where i is the row number of the spreadsheet.
For example:
	
For row i = 1: 				 f(15840) = cGp
For row i = 2:				f(16465) = cmW
For row i = 3:				f(17941) = cX3



Q2 a) First task is to find function f(Ai) using these sets of points in the spreadsheet.

we can use polynomial regression using Numpi and Scipi libraries in python IDE
f = interp1d(A, B, kind='linear')


3.b) Once the f(Ai) is found, what would be the output for the following inputs?
f(30001) = ?
f(55555) = ?
f(77788) = ?

f(30001) = vNx, f(55555) = TxE, and f(77788) = AQ9.



4. The data set on column B corresponds to Column A are unique
   from this largest input will be 79791 and there will be collision or overflow before that limit.
   

