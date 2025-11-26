# Ex.No:4
# Ex.Name:Write a CPP Program to overload the first function to perform addition, second function to perform subtraction, third function to perform multiplication and the fourth function to perform division.
## Date:

## Aim:
To write a C++ program that overloads a function four times to perform addition, subtraction, multiplication, and division.

## Algorithm:
STEP 1: Start the program.

STEP 2: Define a function named calc that accepts two integers and performs addition.

STEP 3: Define an overloaded function calc that accepts two integers and performs subtraction.

STEP 4: Define another overloaded function calc that accepts two integers and performs multiplication.

STEP 5: Define another overloaded function calc that accepts two integers and performs division.

STEP 6: In each overloaded function, compute the correct arithmetic result.

STEP 7: Return the calculated value from each function.

STEP 8: In the main() function, declare two numbers.

STEP 9: Call each overloaded function and display the results.

STEP 10: End the program.




## Program:
```
#include<iostream>
using namespace std;

class mahi
{
    public:
        void Calculate(int n1,int n2)
        {
            cout<<"Sum of two Numbers="<<n1+n2<<endl;
        }
        
        void Calculate(float n1,float n2)
        {
            cout<<"Difference of two Numbers="<<n1-n2<<endl;
        }
        
        void Calculate(double n1,double n2)
        {
            cout<<"Product of two Numbers="<<n1*n2<<endl;
        }
        
        void Calculate(long n1,long n2)
        {
            if(n2!=0)
            {
                cout<<"Division of two Numbers="<<n1/n2<<endl;
            }
            else
            {
                cout<<"no";
            }
        }
};

int main()
{
    int n1,n2;
    cin>>n1>>n2;
    mahi obj1;
    obj1.Calculate(n1,n2);
    
    float a,b;
    cin>>a>>b;
    mahi obj2;
    obj2.Calculate(a,b);
    
    double x,y;
    cin>>x>>y;
    mahi obj3;
    obj3.Calculate(x,y);
    
    long c,d;
    cin>>c>>d;
    mahi obj4;
    obj4.Calculate(c,d);
}
```



## Output:
<img width="969" height="443" alt="{58A50656-7795-423B-AF4D-8961D026A7CF}" src="https://github.com/user-attachments/assets/8d76d62e-71f7-4674-a9ec-47b53ca4f7e2" />



## Result:
Thus, the program successfully demonstrates function overloading by performing addition, subtraction, multiplication, and division using overloaded functions.
