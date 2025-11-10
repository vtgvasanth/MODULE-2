# Ex.No:5
# Ex.Name:Write a CPP Program to overload the first function to perform addition, second function to perform subtraction, third function to perform multiplication and the fourth function to perform division.
## Date:14/08/25

## Aim:
To write a CPP Program to overload the first function to perform addition, second function to perform subtraction, third function to perform multiplication and the fourth function to perform division.


## Algorithm:
1. Start
2. Define a class Calculator with overloaded functions named operation for addition, subtraction, multiplication, and division.
3. Implement the first operation function to add two integers.
4. Implement the second operation function to subtract two floats.
5. Implement the third operation function to multiply two doubles.
6. Implement the fourth operation function to divide two integers with a check for division by zero.
7. In main, create an object of Calculator.
8. Call each overloaded function with appropriate arguments and display results.
9. End


## Program:
```cpp
#include<iostream>
using namespace std;

class Calculate
{
    public:
        
        Calculate(int n1,int n2){
            cout<<"Sum of two Numbers="<<n1+n2<<endl;
        }
        
        Calculate(float n1,float n2){
            cout<<"Difference of two Numbers="<<n1-n2<<endl;
        }
        
        Calculate(double n1,double n2){
            cout<<"Product of two Numbers="<<n1*n2<<endl;
        }
        
        Calculate(long n1,long n2){
            cout<<"Division of two Numbers="<<n1/n2<<endl;
        }
};

int main()
{
    int n1,n2;
    cin>>n1>>n2;
    Calculate obj1(n1,n2);
    float a,b;
    cin>>a>>b;
    Calculate obj2(a,b);
    double x,y;
    cin>>x>>y;
    Calculate obj3(x,y);
    long c,d;
    cin>>c>>d;
    Calculate obj4(c,d);
}
```



## Output:
<img width="1089" height="486" alt="Screenshot 2025-09-08 115023" src="https://github.com/user-attachments/assets/9ff54107-3c3d-4e5c-8c94-03a26389b607" />




## Result:
The program successfully demonstratesthe first function to perform addition, second function to perform subtraction, third function to perform multiplication and the fourth function to perform division.


