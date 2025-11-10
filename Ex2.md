# Ex.No:2
# Ex.Name:Write a CPP Program to overload a function to perform sum of two integers and sum of three integers
## Date:14/08/25

## Aim:
To write a CPP Program to overload a function to perform sum of two integers and sum of three integers


## Algorithm:
1.Start the program.
2.Define a class Addition with two overloaded functions named sum:
3.One function takes two integer arguments and returns their sum.
4.Another function takes three integer arguments and returns their sum.
5.In the main() function, create an object of the class.
6.Call both overloaded functions to compute the sum of two and three integers.
7.Display the results.
8.End the program.





## Program:
```cpp
#include<iostream>
using namespace std;

class Add
{
    public:
        
        
        Add(int n1,int n2){
            cout<<"Sum of two Numbers="<<n1+n2<<endl;
        }
        
        Add(int n1,int n2,int n3){
            cout<<"Sum of three Numbers="<<n1+n2+n3<<endl;
            
        }
};

int main()
{
    int n1,n2;
    cin>>n1>>n2;
    Add obj1(n1,n2);
    int a,b,c;
    cin>>a>>b>>c;
    Add obj2(a,b,c);
}
```



## Output:
<img width="1188" height="437" alt="Screenshot 2025-09-08 111802" src="https://github.com/user-attachments/assets/d61a1ab4-b356-442c-99ef-db54771d7722" />




## Result:
The program successfully demonstrates function overloading by computing the sum of two integers and the sum of three integers using the same function name.


