Print square of a given size. example for 4:
```c
//****
//****  
//****
//****
#include <stdio.h>

int main() {
    int size, i, j;  
    printf("Enter size: ");
    scanf("%d", &size);
    
    for (i = 0; i < size; i++) {   
        for (j = 0; j < size; j++) { 
            printf("*");
        }
        printf("\n"); 
    }
    
    return 0;
}
