# BigIntegers
### An Implementation of BigInteger library in C++

### BigIntegers is a C++ library that is useful when we are dealing with BigIntegers. We can handle big integers (integers having a more significant size than the long long data type). We can perform arithmetic operations like addition, multiplication, subtraction, division, equality check, etc. Also, there are several functions like factorial, reverse. We can check that a number is a palindromic number, counting occurrences, etc. It has some conversion options to convert a string to bhimInteger etc. Overall this library is handy for extensive computing results.


# Usage
#### Download the "BigInteger.h" header .Then #include it inside your code:
```c++
#include "BigInteger.h"   // the actual path may vary
```
# Declaring A Variable
```c++
    BigInteger n1;                                             //n1 defined with value 0
    BigInteger n2(123);                                        //n2 defined with value int value
    BigInteger n3((long long int)1234567898765432);            //n3 defined with value long long int value
    BigInteger n4("7832467326423873423435");                   //n4 defined with string value
    BigInteger n5(n3);   
```

# Converting to BhimNumbers
```c++
    int num1 = -321;
    long long int num2 = -9876543219876543;
    string str1 = "-2112321321321312421534365777";
    BigInteger n6 = to_BigInt(num1);                              //converting int to BigInteger
    BigInteger n7 = to_BigInt(num2);                              //converting long long int to BigInteger
    BigInteger n8 = to_BigInt(str1);                              //converting string to BigInteger
```
 
 # Arithmatic Operations
 ```c++
    cout<<"Addition: "<<n1+n2<<endl;                             //Addition
    cout<<"Subtraction: "<<n2-n1<<endl;                          //subtraction
    cout<<"Multiplication: "<<n1*n2<<endl;                       //Multiplication
    cout<<"Division: "<<n4/n2<<endl;                             //Division

    cout<<"n2 + 5: "<<n2+5<<endl;
    cout<<"n2 - 5: "<<n2-5<<endl;
    cout<<"n2 * 5: "<<n2*5<<endl;
    cout<<"n2 / 5: "<<n2/5<<endl;

    cout<<"5 + n2: "<<5+n2<<endl;
    cout<<"5 - n2: "<<5-n2<<endl;
    cout<<"5 * n2: "<<5*n2<<endl;
    cout<<"5 / n2: "<<5/n2<<endl;
```

# Other Operations

### unary operations
```c++
    cout<<"PreIncrement: "<<++n2<<endl;
    cout<<"PreDecrement: "<<--n2<<endl;
    cout<<"PostIncrement: "<<n2++<<endl;
    cout<<"PostDecrement: "<<n2--<<endl;
```
### equality check
```c++
    cout<<"Check n3 != n5: "<<(bool)(n3 != n5)<<endl;            //Checking if value of both are different
    cout<<"Check n3 == n5: "<<(bool)(n3 == n5)<<endl;            //Checking if value of both are same
```
### few other operators
```c++
    n3 += n2;
    cout<<"n3 += n2: "<<n3<<endl;

    n3 -= n2;
    cout<<"n3 -= n2: "<<n3<<endl;

    n3 *= n2;
    cout<<"n3 *= n2: "<<n3<<endl;

    n3 /= n2;
    cout<<"n3 /= n2: "<<n3<<endl;
```


# Functions
```c++
    cout<<"Maximum: "<<maxBigInt(n1, n2)<<endl;                               //Maximum of two Numbers
    cout<<"Minimum: "<<minBigInt(n1, n2)<<endl;                               //Minimum of two Numbers
    cout<<"absolute: "<<absBigInt(n1)<<" "<<absBigInt(n2)<<endl;                //Absolute value of a number
    cout<<"Factorial: "<<factBigInt(n1)<<" "<<factBigInt(n2)<<endl;             //Factorial of a number
    cout<<"Reverse: "<<revBhim(n3)<<endl;                                   //Reverse a number
    cout<<"Counting the occurance of a digit: "<<countBigInt(n9,6)<<endl;     //Counting the occurance of a digit
    cout<<"Erasing all occurance of a digit: "<<eraseBigInt(n9,4)<<endl;      //Erasing all occurances of a digit
    cout<<"ispaliBigInteger: "<<(bool)ispaliBigInt(n9)<<endl;                       //Checking if a number is palindrome
    cout<<"sorting the digits: "<<sortBigInt(n9)<<endl;                       //sort the digits of a number
	cout<<"Finds power: "<<powBifInt(n3, n2)<<endl;                           //finds x to the power y, where x and y is any int. Returns Integer value in form of string
```
