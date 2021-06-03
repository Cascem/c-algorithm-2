# c-algorithm-2
Cycle algorithm
#define _CRT_SECURE_NO_WARNINGS
#include <stdio.h>
int main() {
	int i=0, n,a,b,c,x;
	scanf("%d", &n);
	if (n < 10)
		n *= 10;
	x = n;
	while (1) {
		a = n / 10;
		b = n % 10;
		c = b*10+(a+b)%10;
		i++;
		if (c == x)
			break;
		n = c;
	}
	printf("%d", i);
	return 0;
}
