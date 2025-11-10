# Ex.No:4
# Ex.Name:Write a CPP Program to Overloadd the '-' operator i.e. a positive value should be turned into a negative value
## Date:14/08/25

## Aim:
To write a CPP Program to Overload the '-' operator i.e. a positive value should be turned into a negative value



## Algorithm:
1. Start
2. Define a class with a data member to store a number.
3. Create a constructor to initialize the number.
4. Overload the unary - operator to change a positive number into its negative.
5. Define a display function to show the number.
6. In main, create an object, display the original value, apply the overloaded - operator, and display the result.
7. End


## Program:
```cpp
#include<iostream>
using namespace std;

class Negate
{
    int n;
    public:
    
        Negate(int a){
            n =a;
        }
        
        void operator -()
        {
            n = -n;
        }
        
        void display(){
            cout<<n<<endl;
        }
};

int main()
{
    int n;
    cin>>n;
    Negate obj(n);
    -obj;
    obj.display();
}
```


## Output:
<img width="1196" height="313" alt="Screenshot 2025-09-08 114537" src="https://github.com/user-attachments/assets/1ee71399-bfed-4651-b3ed-189ebfea85ce" />




## Result:
The program successfully demonstrates to Overload the '-' operator i.e. a positive value should be turned into a negative value





