# Ex.No:1
# Ex.Name:Write A CPP Program to allocate memory dynamically for an integer array. (Note: p_array = new type [size]; )
## Aim:
To write a C++ program to allocate memory dynamically for an integer array using the new operator.

## Algorithm:
STEP 1: Start the program.

STEP 2: Declare a pointer variable to hold the base address of the dynamic array.

STEP 3: Read the size of the array from the user.

STEP 4: Allocate memory dynamically using:
  p_array = new int[size];

STEP 5: Check if memory allocation is successful.

STEP 6: Read elements into the dynamically allocated array.

STEP 7: Display the entered elements.

STEP 8: Perform any operations if required (optional).

STEP 9: Deallocate memory using delete[] p_array;.

STEP 10: End the program.





## Program:
```
#include <iostream>
using namespace std; 

class student {
public:
    double *p_array;
    int size,n;
    student()
    {
        size = 100;
        cout<<"Array Created"<<endl;
        p_array = new double[size];
    }
    ~student()
    {
        cout<<"Array Deleted"<<endl;
        delete[] p_array;
    }
    void createArray()
    {
        cout<<"Array Values :"<<endl;
        cin>>n;
        for(int i=0;i<n;i++){
            cin>>p_array[i];
        }
        
        for(int i=0;i<n;i++){
            cout<<p_array[i]<<" ";
        }
        cout<<"\n";
    }
};

int main()
{
    student obj;
    obj.createArray();
}
```



## Output:
<img width="605" height="334" alt="{550077D0-ACA8-4413-8C44-0C32AB7AC6B2}" src="https://github.com/user-attachments/assets/3fb17ece-6b1f-4b4e-b536-67c721cf5197" />




## Result:
Thus, memory for the integer array is allocated dynamically using the new operator, values are stored and displayed successfully.

