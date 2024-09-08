# Write a C program that finds the largest of three numbers entered by the user.
```C
#include <stdio.h>
main(){
	int a, b, c;
	printf("Enter first number");
	scanf("%d",&a);
	printf("Enter second number");
	scanf("%d",&b);
	printf("Enter third number");      
	scanf("%d",&c);
	printf("Largest Number: ");
	if (a>b && a>c){
		printf("%d",a);
	}
	else
			if (b>c){
				printf("%d",b);
			}
		else
		{
			printf("%d",c);
		}
	
}

