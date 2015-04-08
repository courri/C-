```c
#include "stdio.h"//请给每一行添加注释，随意添加 
long long int fibb(int n);
int main()
{
	printf("下面输出斐波那契数列\n");
	for (int i = 1; i < 20; ++i) {
		printf("%d\n",fibb(i));
	}
	return 0;
}

long long int fibb(int n)
{
	int fnow = 0, fnext = 1, tempf;
	while(--n>0) {
		tempf = fnow + fnext;
		fnow = fnext;
		fnext = tempf;
	}
	return fnext;
}
```
