#include <iostream>

int main() {
    float num1, num2;

    std::cout << "Enter two floating-point numbers separated by space: ";
    std::cin >> num1 >> num2;

    
    float sum = num1 + num2;
    std::cout << "Sum: " << num1 << " + " << num2 << " = " << sum << std::endl;

    
    float difference = num1 - num2;
    std::cout << "Difference: " << num1 << " - " << num2 << " = " << difference << std::endl;

    float product = num1 * num2;
    std::cout << "Product: " << num1 << " * " << num2 << " = " << product << std::endl;

  
    if (num2 != 0) {
        float quotient = num1 / num2;
        std::cout << "Division: " << num1 << " / " << num2 << " = " << quotient << std::endl;
    } else {
        std::cout << "Division by zero is undefined." << std::endl;
    }


    std::cout << "Modulo operation doesn't apply to floating-point numbers." << std::endl;

    return 0;
}
