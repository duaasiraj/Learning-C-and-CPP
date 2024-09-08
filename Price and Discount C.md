## Task:
Write a C program to calculate the discounted price of an item based on original price between
Rs.100 and Rs. 50,000. Discount rate between 5% and 30%. Calculate the final price after
applying the discount. Validate inputs and provide error messages if they are out of range.
Display the final price after discount.
Final Price = Original Price * (1 – Discount Rate / 100)

```C
#include <stdio.h>
main(){
	float originalPrice, Discount, FinalPrice;
	printf("Enter Original Price");
	scanf("%f", &originalPrice);
	printf("Enter Discount");
	scanf("%f",&Discount);
	if (originalPrice<100 || originalPrice>50000){
		printf("Price out of range");
	}	
	else
		if (Discount<5 || Discount>30)
		{
			printf("Discount amount out of range");
		}
		else{
			FinalPrice= originalPrice - (originalPrice*(Discount/100));
			printf("Final Price after discount is: %f",FinalPrice);
		}
}
