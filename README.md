# Cpp-1
#include <iostream>
using namespace std;

int main() {
    char op;
    double num1, num2, result;

    cout<<"Let as calculate the values"<<endl;
    
    cout<<"Enter First numbers: ";
    cin>>num1;
    
    cout<<"Enter the Arithmetic operator(+, -, *, /): ";
    cin>>op;
    
    cout<<"Enter second numbers: ";
    cin>>num2;

    switch(op){
        case '+':
            result=num1 + num2;
            break;
        case '-':
            result=num1 - num2;
            break;
        case '*':
            result=num1 * num2;
            break;
        case '/':
            if (num2 == 0) {
                cout<<"Error: Division by zero is not allowed"<<endl;
                break;
            }
            result=num1/num2;
            break;
        default:
            cout<<"Invalid operator"<<endl;
            return 1;
    }

    cout<<"Result: "<<result<<endl;
    return 0;
}
