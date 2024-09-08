## Write a C program that determines whether a number provided by the user is even or odd.
```C
#include <stdio.h>
main(){
	int num;
	printf("Enter Num: ");
	scanf("%d",&num);
	if (num%2==0){
		printf("Number is even");
	}
	else{
		printf("Number is odd");
	}
}
	
