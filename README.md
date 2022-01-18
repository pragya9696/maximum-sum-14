# maximum-sum-14
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() {
int a[100000],i,sum=0,max=0,n;
      scanf("%d",&n);
    for(i=0;i<n;i++)
        scanf("%d",&a[i]);
  
     for(i=0;i<n;i++)
     {
         sum=sum+a[i];
         if(max<sum)
             max=sum;
         if(sum<0)
             sum=0;
     }
    printf("%d",max);
    /* Enter your code here. Read input from STDIN. Print output to STDOUT */    
    return 0;
}
