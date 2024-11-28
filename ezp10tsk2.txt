/*Aim: WAP to print the elements of an array in Reverse order using pointers.

*/
#include <stdio.h>

int main() {

    int n;

    printf("\t\t** Array Reverser ** \n\n");


    printf("Enter the size of the array: ");
    scanf("%d", &n);

    int arr[n];

    int *ptr = arr;


    printf("Enter the elements of the array:\n");

    for (int i = 0; i < n; i++) {

        scanf("%d", ptr + i);
    }


    printf("\nArray elements in reverse order:\n");

    for (int i = n - 1; i >= 0; i--) {
        printf("%d ", *(ptr + i));
    }

    printf("\n");

    return 0;
}
/*                ** Array Reverser **

Enter the size of the array: 4
Enter the elements of the array:
3
4
4
4

Array elements in reverse order:
4 4 4 3
*/
