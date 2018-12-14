#include <stdio.h>
#include <stdlib.h>
#include <math.h>
int Fibonacci(int n)
{
    int Un;
    if (n==1 || n==2)
    {
        Un=1;
    }
    else {
        Un=Fibonacci(n-1)+Fibonacci(n-2);
    }

    return Un;
}



int main() {
    int n, i=0;

    printf("entrez n\n");
    scanf("%d", &n);
    
    for (i=3; i<=n ; i++){
            printf("%d\n", Fibonacci(i));

    }
    return 0;   
}
