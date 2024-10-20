# Exp-15-Recursion
# Aim
Write a c++ program:
1. To find factorial of a number using recursion.
2. To find fibonacci number in the fibonacci sequence using recursion.
3. To find sum of n natural numbers using recursion.
# Software Used
VS Code and c++ online compiler.
# Theory
Recursion is a programming technique in which a function calls itself directly or indirectly to solve a problem.

Recursion is a powerful technique in C++ programming, enabling the expression of solutions to complex problems in a clear and concise manner. Understanding recursion involves recognizing its structure (base and recursive cases) and its implications on memory and performance.

# Program Code
```
//Factorial using recursion

# include<iostream>
using namespace std;
 int factorial (int n)
{ if ( n == 0)
{
    return 1;
}
else 
{
    return n*factorial(n-1);
    }
    }
    int main()
    {  int num;
       cout<<"Enter a number: "<<endl;
       cin>>num;

       cout<<"The factorial of "<<num<<" is: "<< factorial(num)<<endl;
       return 0;
    }
```
```
//Fibonacci

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
{
    int f,n;
    cout << "Enter number of elements: "<<endl;
    cin >> n ;

    cout << n <<"th Fibonacci number in Fibonacci sequence is: "<<fib(n) ;
}
```
```
//Sum of n natural numbers

# include<iostream>
using namespace std;
int sum(int n)
{
    if(n==0)
    {
        cout<< " Number should be greater than 1"<<endl;
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
    cout << "Enter a number : "<<endl;
    cin >> n ;

    cout << n <<" Sum of numbers from 1 to "<<n<<" is: "<<" : "<<sum(n) ;
}
```

# Output
### Factorial
![image](https://github.com/user-attachments/assets/04b93ecc-4016-498e-80bb-999f6230c56b)
### Fibonacci
![image](https://github.com/user-attachments/assets/bda81dbb-2cf1-4e4a-a35d-5190c9fda05a)
### Sum of n natural numbers
![image](https://github.com/user-attachments/assets/389166d2-680f-4d4d-9966-8e4551e97574)

# Conclusion
We learnt to find factorial, fibonacci sequence and sum of 'n' natural numbers using recursion.

