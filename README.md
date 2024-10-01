#include <stdio.h>
#include <math.h>
int main()
{
    int count =0,n,q=0;
    printf("Enter the number of cases you want\n");
    scanf("%d",&n);
    while(q<n)
    {int list, score, num, d1, d2, d3, d4, d5, d6, d7, d8, d9, d10, avg;
    int  i,d11, d21, d31, d41, d51, d61, d71, d81, d91, d101, scavg;
    int  scoredash,d12, d22, d32, d42, d52, d62, d72, d82, d92, d102;
    
    printf("Enter the number\n");
    scanf("%d", &num);
    list = pow(10, num) - 3;
  
    d1 = list % 10;
    d2 = (list / 10) % 10;
    d3 = (list / 100) % 10;
    d4 = (list / 1000) % 10;
    d5 = (list / 10000) % 10;
    d6 = (list / 100000) % 10;
    d7 = (list / 1000000) % 10;
    d8 = (list / 10000000) % 10;
    d9 = (list / 100000000) % 10;
    d10 = (list / 1000000000) % 10;
    score = d1 + d2 + d3 + d4 + d5 + d6 + d7 + d8 + d9 + d10;
   

    avg = (1 + list) / 2;
   
    d11 = avg % 10;
    d21 = (avg / 10) % 10;
    d31 = (avg / 100) % 10;
    d41 = (avg / 1000) % 10;
    d51 = (avg / 10000) % 10;
    d61 = (avg / 100000) % 10;
    d71 = (avg / 1000000) % 10;
    d81 = (avg / 10000000) % 10;
    d91 = (avg / 100000000) % 10;
    d101 = (avg / 1000000000) % 10;
    scavg=d11+d21+d31+d41+d51+d61+d71+d81+d91+d101;
   
    for ( i = 1; i <= list; i++)
    {
        d12=i%10;
        d22=(i/10)%10;
        d32=(i/100)%10;
        d42=(i/1000)%10;
        d52=(i/10000)%10;
        d62=(i/100000)%10;
        d72=(i/1000000)%10;
        d82=(i/10000000)%10;
        d92=(i/100000000)%10;
        d102=(i/100000000)%10;
        scoredash=d12+d22+d32+d42+d52+d62+d72+d82+d92+d102;
        
        if (scoredash>scavg)
        {
            count++;
        }
        
        

    }
    printf("the total number of numbers from the list is %d\n",count);
    count =0;
    q++;
    }
    
   
    
    return 0;
}
