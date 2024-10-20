# Task: Transpose of a 4 by 4 matrix
```
EG:
Enter element for 0 01
Enter element for 0 12
Enter element for 0 23
Enter element for 0 34
Enter element for 1 05
Enter element for 1 16
Enter element for 1 27
Enter element for 1 38
Enter element for 2 09
Enter element for 2 10
Enter element for 2 21
Enter element for 2 32
Enter element for 3 03
Enter element for 3 14
Enter element for 3 25
Enter element for 3 36
Original array
 1 	 2 	 3 	 4 	
 5 	 6 	 7 	 8 	
 9 	 0 	 1 	 2 	
 3 	 4 	 5 	 6 	

Transpose array
 1 	 5 	 9 	 3 	
 2 	 6 	 0 	 4 	
 3 	 7 	 1 	 5 	
 4 	 8 	 2 	 6 	
```
# Solution:
```c

#include <stdio.h>

int main() {
    int array2d[4][4];
    for (int i=0;i<4;i++){
        for (int j=0;j<4;j++){
            printf("Enter element for %d %d",i,j);
            scanf("%d",&array2d[i][j]);
        }
    }
    printf("Original array\n");
    for (int k=0;k<4;k++){
        for (int m=0;m<4;m++){
            printf(" %d \t",array2d[k][m]);
        }
        printf("\n");
    }
    int trans[4][4];
        for (int n=0;n<4;n++){
        for (int o=0;o<4;o++){
            trans[o][n]=array2d[n][o];
        }
        }
    printf("\nTranspose array\n");
    for (int p=0;p<4;p++){
        for (int q=0;q<4;q++){
            printf(" %d \t",trans[p][q]);
        }
        printf("\n");
    }
    

}
