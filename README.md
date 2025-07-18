# mathematical-operations
#include <iostream>
<br>
using namespace std;
<br>

int sum(int a, int b) {
    <br>
    return a + b;
    <br>
}
<br>
int product(int a, int b) {
    <br>
    return a * b;
    <br>

}
<br>

int factorial(int n) {
    <br>
    int res = 1;
    <br>
    for (int i = 1; i <= n; i++) {
        <br>
        res *= i;
        <br>
    }
    <br>
    return res;
    <br>
}
<br>
void divide(int a, int b) {
    <br>
    if (b == 0) {<br>
        cout << "Error: Division by zero!" << endl;
        <br>
    } else {
        <br>
        double result = (double)a / b;<br>
        cout << "Division result = " << result << endl;<br>
    }<br>
}<br>

int main() {<br>
    int a, b, n;
<br>
    cout << "Enter first number: ";<br>
    cin >> a;<br>
    cout << "Enter second number: ";<br>
    cin >> b;<br>
    cout << "Enter number for factorial: ";<br>
    cin >> n;<br>

    cout << "Sum = " << sum(a, b) << endl; 
    <br>
    cout << "Product = " << product(a, b) << endl; 

    <br>
    divide(a, b);
    <br>
    cout << "Factorial = " << factorial(n) << endl;
<br>
    return 0;
    <br>
}