# dayOfyear
a simple code
#include<stdio.h>

int main ()
{
	int i = 0;
	for(i=100;i<=200;i++)
	{
		if(is_prime(i) == 1)
		{
			printf("%d",i);
		}
	}
}
int is_prime(int i)
{
	while(j!=sqrt(i))
	{
		int j=2;
		if(i%j==0) 
			j++;
		else return 0;
	}
	return 1;
}
