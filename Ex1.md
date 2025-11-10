# Ex.No:1
# Ex.Name:Write a CPP program to overload the (+) operator to add two objects both the objects will have the details of a Box i.e their height, length, breadth, and calculate their volume and then using the overloaded operator Add the length, breadth and height of the two objects and store into another object and calculate the volume of the third object.
## Date:14/08/25

## Aim:
To write a CPP program to overload the (+) operator to add two objects both the objects will have the details of a Box i.e their height, length, breadth, and calculate their volume and then using the overloaded operator Add the length, breadth and height of the two objects and store into another object and calculate the volume of the third object.


## Algorithm:
1. Start
2. Define a class Box with data members: length, breadth, height.
3. Add a constructor to initialize these values.
4. Define a function calculateVolume() that returns length * breadth * height.
5. Overload the + operator to add the length, breadth, and height of two Box objects and return a new Box object.
6. In main():Create two objects (Box1 and Box2) with some values.
7. Display their dimensions and volumes.
8. Use the overloaded + operator to add Box1 and Box2 → store result in Box3.
9. Display dimensions and volume of Box3.
10. End.

## Program:
```cpp
#include<iostream>
using namespace std;
class box
{
    public:
    float length,breadth,height;
    float Volume()
    {
        float volume;
        volume=length*breadth*height;
        return volume;
    }
    box operator+(box b4)
    {
        box b5;
        b5.length=length+b4.length;
        b5.breadth=breadth+b4.breadth;
        b5.height=height+b4.height;
        return b5;
    }
    
};
int main()
{
    float vol;
    box b1,b2,b3;
    cin>>b1.length>>b1.breadth>>b1.height;
    cin>>b2.length>>b2.breadth>>b2.height;
    b3=b1+b2;
    vol=b1.Volume();
    cout<<"Volume of Box1 : "<<vol<<endl;
    vol=b2.Volume();
    cout<<"Volume of Box2 : "<<vol<<endl;
    vol=b3.Volume();
    cout<<"Volume of Box3 : "<<vol<<endl;
}


```



## Output:
<img width="1188" height="437" alt="Screenshot 2025-09-08 111802" src="https://github.com/user-attachments/assets/52f1d4d7-949f-44dc-a4c1-27a2dc84109a" />


## Result:
The program successfully demonstrates function overloading operator Add the length, breadth and height of the two objects and store into another object and calculate the volume of the third object.

