## Task :
Write a C program to calculate the volume of a cylinder given its radius and height. Use the
formula: Volume = π r^2 h where π is approximately 3.14159. Format the result to 3 decimal places.

```C
#include <stdio.h>
main(){
	float radius,height,Volume;
	float pi = 3.14159;
	printf("Enter Radius:");
	scanf("%f",&radius);
	printf("Enter Height");
	scanf("%f",&height);
	Volume = pi*radius*radius*height;
	printf("Volume is %.3f" , Volume);
}
	
