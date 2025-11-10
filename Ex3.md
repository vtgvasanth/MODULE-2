# Ex.No:3
# Ex.Name:Write A CPP Program to create class Rectangle and calculate the volume of the rectangle, make use of static member variable in the class Rectangle.
## Date:14/08/25

## Aim:
To write A CPP Program to create class Rectangle and calculate the volume of the rectangle, make use of static member variable in the class Rectangle.


## Algorithm:
1. Start
2. Define a class Rectangle with data members length and breadth, and a static data member count.
3. Create a constructor to initialize length and breadth and increment count whenever a new object is created.
4. Define a function to calculate area as length × breadth.
5. Define a function to calculate volume as length × breadth × height.
6. Define a static function to return the value of count.
7. In main, create Rectangle objects, calculate and display their area and volume, and display the total number of objects created using the static member.
8. End



## Program:
```cpp
#include <iostream>
 
using namespace std;

class Square {
    public:
        static int count;
      
      // Constructor definition
      Square(double l,double b,double h) 
      {
          cout<<"Constructor called."<<endl;
          length = l;
          breadth = b;
          height = h;
          count++;
      }
      double Volume() 
      {
        return length*breadth*height;
      }
      
   private:
      double length;     // Length of a box
      double breadth;    // Breadth of a box
      double height;     // Height of a box
};
int Square::count;
int main(void) 
{
    double l,b,h;
    cin>>l>>b>>h;
   Square obj1(l,b,h);
   cout<<"Volume :"<<obj1.Volume()<<endl;
   cin>>l>>b>>h;
   Square obj2(l,b,h);
   cout<<"Volume :"<<obj2.Volume()<<endl;
   cout<<"Total objects: "<<Square::count<<endl;
   return 0;
}
```



## Output:
<img width="1188" height="437" alt="Screenshot 2025-09-08 111802" src="https://github.com/user-attachments/assets/e7c2e7af-5523-471c-8db0-7d863e83c1ac" />




## Result:
The program successfully created class Rectangle and calculate the volume of the rectangle, make use of static member variable in the class Rectangle.

