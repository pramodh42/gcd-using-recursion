# gcd-using-recursion


#include<stdio.h>

unsigned int  gcd(unsigned int,unsigned int, unsigned int);

int main()

{

unsigned int num1,num2,value,j; 

printf("enter  positive numbers which is to be checked");

scanf("%u%u",&num1,&num2); 

j=num1<num2?num1:num2;

value=gcd(num1,num2,j); 

printf("gcd is %u",value); 

}

unsigned int  gcd(unsigned int m,unsigned int n, unsigned int j)

{  

 if(j==1) 

 return j; 

else 

 { if(m%j==0&&n%j==0)  

   return j;

   else 

   return gcd(m,n,j-1); 

  } 

}

  
