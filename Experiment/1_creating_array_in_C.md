// Online C compiler to run C program online
#include <stdio.h>
#include <stdlib.h>

int main() {


    int a = 50;           // Created a int type vlaue
    int *add = &a;        // Get its address
    printf("%p \n",add);   // printed Address
    printf("%d \n",*add);     // printed value at address
    
    int n = 10;
    int *arr =  (int*)malloc(n * sizeof(int));
    printf("%p \n",arr);
    for(int i=0;i<n;i++){
      int *current_add =  arr + i * sizeof(int);
      *current_add = i *i;
    }
    
    for(int i=0;i<n;i++){
      int *current_add =  arr + i * sizeof(int);
      printf("%d \n",*current_add);
    }
    
    

    return 0;
}

![image](https://github.com/user-attachments/assets/c7cd8538-7729-43f3-8fde-8014b17ac96d)





