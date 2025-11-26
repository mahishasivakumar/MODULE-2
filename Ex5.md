# Ex.No:5
# Ex.Name:Write a CPP Program to overload the Operator (++) i.e. on invoking it the incrementation should happen by some random value.
## Date:
## Aim:
To write a C++ program to overload the increment operator (++) so that whenever it is invoked, the value increases by a random value instead of just 1.

## Algorithm:
STEP 1: Start the program.

STEP 2: Create a class Increment.

STEP 3: Declare a private data member to store a number.

STEP 4: Define a constructor to initialize the number.

STEP 5: Overload the operator ++ using a member function.

STEP 6: Inside the overloaded operator function, generate a random value using rand().

STEP 7: Add the random value to the data member.

STEP 8: Return the modified object.

STEP 9: In main(), create an object and apply the overloaded ++ operator.

STEP 10: Display the updated value and end the program.




## Program:
```
#include<iostream>
using namespace std;

class Add
{
    private:
        int n1,n2;
        
    public:
    
        Add(int a,int b)
        {
            n1 = a;
            n2 = b;
        }
        
        void operator ++()
        {
            n1 = n1+n2;
        }
        
        void display()
        {
            cout<<n1<<endl;
        }
};


int main()
{
    int n1,n2;
    cin>>n1>>n2;
    Add obj(n1,n2);
    ++obj;
    obj.display();
}
```


## Output:
<img width="527" height="328" alt="{4A921AFC-E781-4957-BD15-330F60207BAE}" src="https://github.com/user-attachments/assets/1d4712ab-66b1-489d-bb2c-68b2f2ac8534" />




## Result:
Thus, the overloaded operator (++) increments the value by a random amount when invoked.

