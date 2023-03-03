# dayOfyear
a simple code
#include<stdio.h>
#include<stdlib.h>
int main() {
int i;//water flower number 
int x, y, z;
for (i = 100; i < 999; i++)
{
x = i / 100;
y = i / 10 % 10;
z = i % 10;
if (i == x * x * x + y * y * y + z * z * z)
{
printf("%-3d\n", i);
}
}
	
