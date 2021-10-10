# Calculator
#include <stdio.h>
int main()
{
int i;
for(;;)
{
double a, b;
printf("Enter two operands: \n");
scanf("%lf %lf", &a, &b);
char op;
printf("Enter an operator (+, -, *, /): ");
scanf("%s",&op);
switch (op)
{
case '+':
printf("%lf + %lf = %lf",a,b,a + b);
break;
case '-':
printf("%lf - %lf = %lf",a,b,a-b);
break;
case '*':
printf("%lf * %lf = %lf", a,b,a*b);
break;
case '/':
printf("%lf / %lf = %lf",a,b,a/b);
break;
default:
printf("Error! operator is not correct");
}
printf("\nEnter 1 to continue else any other number to exit: ");
scanf("%d",&i);
if(i!=1)
{
break;
}
}
}
