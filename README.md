//# Armstrong-number.c//
#include<stdio.h>
int main()
{
    int n,rem,t,arm=0;
    printf("Enter a three digit number");
    scanf("%d",&n);
    t=n;
    while(n>0)
    {
        rem=n%10;
        arm=(rem*rem*rem)+arm;
        n=n/10;
    }
    if(t==arm)
    {
        printf("%d is armstrong",t);
    }
    else
    {
        printf("%d is not armstrong",t);
    }
    return 0;
}
