# Recursion in C++

## AIM
To learn about recursion in C++.

## Problem Statement
1. **Factorial:** Write a C++ program to calculate the factorial of a number using recursion.
2. **Fibonacci Sequence:** Write a C++ program to find the Fibonacci number in the Fibonacci sequence using recursion.
3. **Sum of Natural Numbers:** Write a C++ program to find the sum of the first `n` natural numbers using recursion.

## Theory
Recursion is a technique where a function calls itself. This approach allows complex problems to be broken down into simpler, more manageable problems. Understanding recursion can be challenging, but experimentation is key to grasping how it works.

## Program Codes
```javascript
//Mukesh Rothe 23070123089
# include<iostream>
using namespace std;
 int factorial (int n)
{ if ( n == 0)
{ return 1;
}
else 
{   return n*factorial(n-1);
    }
    }
    int main()
    {  int num;
       cout<<"Enter a number- "<<endl;
       cin>>num;
       cout<<"The factorial of "<<num<<" is- "<< factorial(num)<<endl;
       return 0;
    }
```
```javascript
//Mukesh Rothe 23070123089
# include<iostream>
using namespace std;
int fib(int n)
{
if(n==0)
    {
        return 0;
    }
if(n==1)
    {
        return 1;
    }
 else
    {
     return (fib(n-1) + fib(n-2));
    }
}
int main()
{   int f,n;
    cout << "Enter number of elements: "<<endl;
    cin >> n ;
    cout << n <<"th Fibonacci number in Fibonacci sequence is: "<<fib(n) ;
}
```
```javascript
//Mukesh Rothe 23070123089
# include<iostream>
using namespace std;
int sum(int n)
{
    if(n==0)
    {
        cout<< "Number should be greater than 1"<<endl;
    }
    if(n==1)
    {
        return 1;
    }
    else
    {
     return (n+sum(n-1));

    }
}
    int main()
{
    int f,n;
    cout << "Enter a number- "<<endl;
    cin >> n ;
    cout<<"Sum of numbers from 1 to "<<n<<" is- "<<" : "<<sum(n) ;
}
```
## Output
Factorial-

![Screenshot 2024-10-03 211240](https://github.com/user-attachments/assets/6eed13d8-f5c8-4724-b94a-4c718f9f511c)

Fibonacci-

![Screenshot 2024-10-03 211442](https://github.com/user-attachments/assets/16cf54a6-a63e-485c-bf9f-fcd50c5fd7e4)

Sum of 'n' natural numbers-

![Screenshot 2024-10-03 211714](https://github.com/user-attachments/assets/06e51111-620f-4016-af85-9700c4abbe21)

## Conclusion
We learned to compute the factorial, generate the Fibonacci sequence, and calculate the sum of `n` natural numbers using recursion.
