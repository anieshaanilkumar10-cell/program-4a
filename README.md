# program-4a
#include<stdio.h>
#include<stdlib.h>
int gcd(int a,int b)
{
    if(b!=0)
    {
        return gcd(b,a%b);
    }
    else
    {
        return a;
    }
}
int main()
{

    int a,b;
    printf("\nRead two numbers:");
    scanf("%d %d",&a,&b);
    printf("\nGCD of %d",&a,&b);
    printf("\nGCD of %d and %d is %d\n",a,b,gcd(a,b));
    return 0;
}

