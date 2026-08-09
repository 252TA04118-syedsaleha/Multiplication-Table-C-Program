#include <stdio.h>

int main() {
    int number, start, end, i, result;

    printf("=====================================\n");
    printf("       MULTIPLICATION TABLE         \n");
    printf("=====================================\n");

    printf("\nEnter the number: ");
    scanf("%d", &number);

    printf("Enter starting value: ");
    scanf("%d", &start);

    printf("Enter ending value: ");
    scanf("%d", &end);

    printf("\n=====================================\n");
    printf("       TABLE OF %d                  \n", number);
    printf("=====================================\n");

    for (i = start; i <= end; i++) {
        result = number * i;
        printf("%d x %d = %d\n", number, i, result);
    }

    printf("\n-------------------------------------\n");
    printf("          TABLE INFORMATION          \n");
    printf("-------------------------------------\n");

    if (number % 2 == 0) {
        printf("%d is an even number.\n", number);
    } else {
        printf("%d is an odd number.\n", number);
    }

    printf("\nThe multiplication table was generated successfully.\n");

    printf("\n=====================================\n");
    printf("        Program Completed!           \n");
    printf("=====================================\n");

    return 0;
}
