# dayOfyear
a simple code
#include<stdio.h>

int main()
{
	int num, n;
	int count = 1;
	long int tnum = 0, tn = 0;
	printf("Please input number and bit:\n");
	scanf("%d %d", &num, &n);
	while (count <= n)
	{
		if (tn != 0) printf("+");
		tn = tn + num;//2  22  222
		tnum = tnum + tn;//2+22+222+...
		num = num * 10;//200
		++count;
		printf("%d", tn);
	}
	printf("=%d", tnum);
	return 0;
}
