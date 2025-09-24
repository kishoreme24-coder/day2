#include <stdio.h>
#include <math.h> // Required for sqrt()

// Function to check if a number is prime
int isPrime(int n) {
    if (n <= 1) {
        return 0; // 0 and 1 are not prime numbers
    }
    if (n == 2) {
        return 1; // 2 is the only even prime number
    }
    if (n % 2 == 0) {
        return 0; // Other even numbers are not prime
    }

    // Check for divisibility from 3 up to the square root of n,
    // incrementing by 2 to check only odd divisors
    for (int i = 3; i * i <= n; i += 2) {
        if (n % i == 0) {
            return 0; // If divisible, it's not prime
        }
    }
    return 1; // If no divisors found, it's prime
}

int main() {
    int num;
    printf("Enter a number: ");
    scanf("%d", &num);

    if (isPrime(num)) {
        printf("%d is a prime number.\n", num);
    } else {
        printf("%d is not a prime number.\n", num);
    }

    return 0;
}
