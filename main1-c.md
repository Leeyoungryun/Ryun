# Ryun

#include <stdio.h>

int add(int, int);
int sub(int, int);
int div(int, int);
int multi(int, int);

int _tmain(int argc, char * argv[])
{
	int a, b, c;
	int number, number2, result;
	char Operator;

	printf("Please enter a expression");
	printf("Please enter a expression: ");
	scanf("%d %d %d", &a, &Operator, &b);

	switch(Operator)
	{
	case '+':
		c= add(a,b);
		break;
	case '-':
		c = sub(a,b);
		break;
	case '*':
		c = multi(a,b);
		break;
	case '/':
		c = div(a,b);
		break;
	}
	return 0;
}

