Task:
Create a pattern as follows for any size, the given one is 5:
```
     *
    ***
   *****
  *******
 *********
***********
  .......
   .....
    ...
     .
```
Solution
```c
#include <stdio.h>

int main() {
    int size;
    printf("Enter size");
    scanf("%d",&size);
    int space=size-1;
    for (int i=0;i<=size;i++){
        for (int j=0;j<=space;j++){
            printf(" ");
        }
        space--;
        for(int k=1;k<=2*i+1;k++){
            printf("*");
        }
        printf("\n");
    }
    space=1;
    for(int m=0;m<=size;m++){
        for (int n=0;n<=space;n++){
            printf(" ");
        }
        space++;
        for(int o=2*m-1;o<=size;o++){
            printf(".");
        }
        printf("\n");
    }
    return 0;
}
