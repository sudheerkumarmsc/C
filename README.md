# C
C programs 


#include<stdio.h>

int AddOne(int );

int main(void)
{
    int Num=10;
    
    printf("%d\n",AddOne(Num));
    return 0;
}

int AddOne(int x)
{
  int m=1;
  
  while(x&m)
  {
    x = x&(~m);
    m<<=1;
  }
  
  x = x | m;
  return x;
}
