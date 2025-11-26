# Ex.No:2
# Ex.Name:Write A CPP Program to create class RectangleBox and calculate the volume of the rectangleBox use of static member variable and static member function in the class RectangleBox.
## Date:

## Aim:
To write a C++ program to create a class RectangleBox and calculate the volume of the box using a static member variable and static member function.


## Algorithm:
STEP 1: Start the program.

STEP 2: Create a class named RectangleBox.

STEP 3: Declare three non-static data members: length, breadth, height.

STEP 4: Declare a static member variable volume to store the calculated volume.

STEP 5: Create a member function to read the dimensions (length, breadth, height).

STEP 6: Create a static member function calculateVolume() to compute volume using:
  volume = length × breadth × height.

STEP 7: In the static function, access the passed object to read dimensions.

STEP 8: Display the calculated volume inside the static function or through another function.

STEP 9: In the main() function, create an object of the class and call required functions.

STEP 10: End the program.


## Program:
```
#include <iostream>
using namespace std;
class Square
{
private:
    static int count;
    int l,b,h;
public:
    Square(int x,int y,int z)
    {
        count++;
        cout << "Constructor called." <<endl;
        l=x;
        b=y;
        h=z;
    }
    void calculateVolume() 
    {
        cout<<"Volume :"<<l*b*h<<endl; 
    }
    
    static int getCount() 
    {
        return count;
    }
};

int Square::count = 0;

int main()
{
    int l, b, h;
    
    cout << "Inital Stage Count: " << Square::getCount() <<endl;
    
    cin >> l>>b>>h;
    Square obj1(l,b,h);
    obj1.calculateVolume();
    
    cin >> l>>b>>h;
    Square obj2(l,b,h);
    obj2.calculateVolume();
    
    cout << "Total objects: " << Square::getCount() <<endl;
    cout << "Final Stage Count: " << Square::getCount() << endl;
    
    return 0;
}

```



## Output:
<img width="723" height="491" alt="{6A97E6F3-9991-4011-B4EF-542E14ECDC0D}" src="https://github.com/user-attachments/assets/f3c4c726-6eb0-4a7c-ad56-2797b3409cdb" />



## Result:
Thus, the program successfully demonstrates the use of static member variable and static member function to calculate the volume of a RectangleBox.
