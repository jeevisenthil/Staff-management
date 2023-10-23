# Staff-management
C program code for Staff Management Database
```
#include <stdio.h>
#include <string.h>

struct Stock {
    char name[50];
    float price;
    int quantity;
};

int main() {
    struct Stock stocks[100]; // Array to store stock information
    int numStocks; // Number of stocks in the array

    // Input stock information
    printf("Enter the number of stocks: ");
    scanf("%d", &numStocks);

    for (int i = 0; i < numStocks; ++i) {
        printf("Enter stock name: ");
        scanf("%s", stocks[i].name); // Assume stock names do not contain spaces
        printf("Enter stock price: ");
        scanf("%f", &stocks[i].price);
        printf("Enter stock quantity: ");
        scanf("%d", &stocks[i].quantity);
    }

    // Display stock information
    printf("\nStock Information:\n");
    for (int i = 0; i < numStocks; ++i) {
        printf("Stock Name: %s\n", stocks[i].name);
        printf("Stock Price: %.2f\n", stocks[i].price);
        printf("Stock Quantity: %d\n", stocks[i].quantity);
    }

    return 0;
}
```
