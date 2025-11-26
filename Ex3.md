# Ex.No:3
# Ex.Name:Write a CPP Program to overload a function to perform sum of two integers and sum of three integers
## Date:

## Aim:
To write a C++ program to overload a function that performs the sum of two integers and the sum of three integers.


## Algorithm:
STEP 1: Start the program.

STEP 2: Create a function named sum with two integer parameters.

STEP 3: Inside the function, compute the sum of the two integers.

STEP 4: Return the calculated result.

STEP 5: Create another overloaded function named sum with three integer parameters.

STEP 6: Inside this function, compute the sum of the three integers.

STEP 7: Return the calculated result.

STEP 8: In the main() function, declare variables to store values.

STEP 9: Call the appropriate overloaded function based on number of arguments and display the results.

STEP 10: End the program.




## Program:
```
#include<iostream>
using namespace std;

class mahi
{
    public:
        
        void Addd(int n1,int n2)
        {
            cout<<"Sum of two Numbers="<<n1+n2<<endl;
        }
        
        void Addd(int n1,int n2,int n3)
        {
            cout<<"Sum of three Numbers="<<n1+n2+n3<<endl;
            
        }
};

int main()
{
    int n1,n2;
    cin>>n1>>n2;
    mahi obj1;
    obj1.Addd(n1,n2);
    
    int a,b,c;
    cin>>a>>b>>c;
    mahi obj2;
    obj2.Addd(a,b,c);
    
}
```


## Output:
<img width="884" height="316" alt="{8BE21FD1-786E-40DB-A2CD-490FF8D90903}" src="https://github.com/user-attachments/assets/e2e089b8-0b24-41d3-8ef8-f4592e1abe4d" />




## Result:
Thus, the program successfully demonstrates function overloading by calculating the sum of two integers and the sum of three integers.

