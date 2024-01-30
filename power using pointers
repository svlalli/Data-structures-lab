#include <stdio.h>

double power(double base, double exponent);

int main() {
    double base, exponent;
    printf("Enter the base number: ");
    scanf("%lf", &base);
    printf("Enter the exponent: ");
    scanf("%lf", &exponent);
    double (*power_ptr)(double, double) = &power;
    double result = (*power_ptr)(base, exponent);
    printf("%.2lf^%.2lf = %.2lf", base, exponent, result);
    return 0;
}

double power(double base, double exponent) {
    double result = 1.0;
    while (exponent > 0) {
        result *= base;
        --exponent;
    }
    return result;
}

