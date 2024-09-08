## A travel agency asks you to develop a program in C that can convert an amount from one currency to another. The user should input the amount in their local currency and theconversion rate for the desired foreign currency. The program should then output the equivalent amount in the foreign currency.
```C
#include <stdio.h>
main(){
	float original, conversionrate, converted;
	printf("Enter the original amount:");
	scanf("%f",&original);
	printf("Enter the Conversion Rate of the desired currency:");
	scanf("%f",&conversionrate);
	converted = original*conversionrate;
	printf("New amount will be: %f", converted);
}
