    #include <stdio.h>


    int recursiveSum(int *n) {
    if (*n == 0) {
        return 0; 
    } else {
        int current = *n;       
        (*n)--;     
        return current + recursiveSum(n);  
    }
    }

    int main() {
    int num = 10;   
    int *ptr = &num; 

    int sum = recursiveSum(ptr);

    printf("Sum of first 10 numbers = %d\n", sum);

    return 0;
    }
