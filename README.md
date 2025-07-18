# mathematical-operations
#include <iostream>
using namespace std;


int sum(int a, int b) {
    return a + b;
}

int product(int a, int b) {
    return a * b;
}

int factorial(int n) {
    int res = 1;
    for (int i = 1; i <= n; i++) {
        res *= i;
    }
    return res;
}

void divide(int a, int b) {
    if (b == 0) {
        cout << "Error: Division by zero!" << endl;
    } else {
        double result = (double)a / b;
        cout << "Division result = " << result << endl;
    }
}

int main() {
    int a, b, n;

    cout << "Enter first number: ";
    cin >> a;
    cout << "Enter second number: ";
    cin >> b;
    cout << "Enter number for factorial: ";
    cin >> n;

    cout << "Sum = " << sum(a, b) << endl;
    cout << "Product = " << product(a, b) << endl;
    divide(a, b);
    cout << "Factorial = " << factorial(n) << endl;

    return 0;
}