hi# C++-language-
Program language oops

class= class is the user defined data type or blue print that wrapped data and functions in to the single entity.

syntax= class classname{
                    data
                      +
                  function};
                  
object= object is a contract representation of the blue print that is defined by the class.

Ex #include<iostream>
using namespace std;
class person {
private:
    int age;
    string name;
    string address;
public:
    void input() {
        cout << "Enter the age: ";
        cin >> age;
        cin.ignore(); // to ignore newline after age input
        cout << "Enter the name: ";
        getline(cin, name); // to read full name

        cout << "Enter the address: ";
        getline(cin, address); // to read full address
    }
    void show() {
        cout << "Age: " << age << endl;
        cout << "Name: " << name << endl;
        cout << "Address: " << address << endl;
    }
};
int main() {
    person ak, raj, rk;

    cout << "Enter details for AK:\n";
    ak.input();
    ak.show();

    cout << "\nEnter details for Raj:\n";
    raj.input();
    raj.show();

    cout << "\nEnter details for RK:\n";
    rk.input();
    rk.show();

    return 0;
}

# Features of oops
*Encapsulation 
*Inheritance 
*Abstraction 
*Polymorphism 
*Class & Object 

ENCAPSULATION 

In it we use binding Data and mention with in the class providing control over the accebality and it prevents external code from directly modifing the internal code of an object.

syntax 
      class person:
      {
      private:
      data:
      public:
      function ()
      };


EX

#include <iostream>
using namespace std;
  class Encap{
  public:
  int age;
  string name;
  };
  int main (){
  Encape E;
  E.age=22;
  E.name="AK"
  cout<<E.age<<endl<<E.name;
  }


# TOKENS 

Smallest individual unit in a program.

It has 6 type 
*Keywords 
*Identifies 
*Constant 
*Data type
*Operator 


1.KEYWORD 
   . Expressively is a identifier is and can't  be used as name for program variables or other user defined program elements 
   . There are 32 key words
   .They have predefined meaning which can't be changed 
   Ex=  brak,goto,int,if, while,etc.

2.Identifier 
 It refors to the name of variables, function, array,class.


 Rules 
 1.Only alphabetical chart degits and '_' underscores are committed.

 2. Name can't start with digit.

 3. Upper case and lower case letters are disting.

 4. Keyword can't be used as variables name.

ex =ARRAY

Constant 
1.Constant refors to fixed value 
2.It value don't change during execution of program.

ex= AREA OF CIRCLE= πR×R (R= Radius of circle,π=3.14)


Operator 
It is a symbol used to perform a mathematical or logical maneculations 

Type of operator 

1. Assigment operator
2. Arithmetic operator
3. Logical operator
4. Relational operators
5. Increament and Decrement operator
6. Bitwise operators


Code


#include<iostream>
using namespace std;
int main (){
int a= 6 ;
int b=9 ;
if (a>b){
cout <<"A is greater";
}
else{
cout<<" b is greater";
}
}


 # Data type 
Data type define the type of data a variable can hold. There are 3 type of data type in C++.

1. Primary data type
2. Derived data type
3. user defined data type


1.Primary data type

Primary data types that allow programmers to store and manipulate different kinds of data effectively.


1.Integer
 
2.Character

3.Hosting point 

4.Double
 
5.Void.

6.Boolean 



2 Derived data type 


A derived data type is a data type that is created from one or more existing data types. Derived data types can be used to create more complex structures that can hold multiple values or different types of data.

1.Function 

2.Array 

3.Pointer
 
4.Reference
 


3 Users defined data type 

A user-defined data type (UDT) is a data type that is defined by the user rather than being built into the programming language. User-defined data types allow programmers to create complex data structures that can better represent real-world entities and relationships. 

1.Class

2.Structure
 
3.Union 

4.Exum

5.Type def

code

#include <iostream>
using namespace std;

int main (){
int a=10;
cout<<"Integer type a"=<<a<<"\n";
cout<<"size of integer=<<size of integer<<
flaot b=34.84
cout<<"float"type b=<<b<<"\n"
double d=34.67
cout <<"double types d=<<d<<"\n";
}

# condition statement 

Conditional statement allow you to make a desigion based on the result of condition .

Type of condition statement  

1.If statement 

Only one condition is present in the program

2.If....else statement 

Two condition are present in the program

3.If....else....if statement

More then one conditin are present in the program 

4.Nested..if statement 

In if condition one more if condition is present

5.Switch statement

It is nothing but multiple choice selection statement it means when we want to select one case outoff multiple case 

*Syntax 


1.If...statement

= if condition 
{
//statement;
}


#include<iostream>
using namespace std;
int main (){
    string signal;
    cout<<"enter the weather condition:";
    cin>>signal;
    if (signal =="red"){
        cout<<"dont go ! plz wate";
    }
    if (signal=="green"){
    
        cout<<"Dont stop you can go";
        
    }
}



#include<iostream>
using namespace std;
int main (){
    string signal;
    cout<<"Enter the signal value ";
    cin>>signal;
    if (signal=="red"){
        cout<<"don't go ! plz stop "<<endl;
        cout<<"if it green you can go";
    }    
}


2. If....else

If...statement

= if condition 
{
//statement;
}If...statement

else
{
//statement;
}
   

#include<iostream>
using namespace std;
int main (){
    string weather;
    cout<<"Enter the weather condition ";
    cin>>weather;
    if (weather=="raining"){
        cout<<"need an umbralla to go out "<<endl;
    }
    else
    {
        cout<<"Don't  need an umbralla";
    }
}


3.If...else...if..


= if condition 
{
//statement;
}

else if condition 
{
//statement;
}

else if condition 
{
//statement;
}

 else 
{
//statement;
}


#include<iostream>
using namespace std;
int main (){
    int amt,tax;
    cout<<"enter the amount:";
    cin>>amt;
    if (amt <= 10000){
        cout<<"don't need t pay tax ";
    }
     else if (amt>10000&& amt==50000){
       tax=amt*10/100;
        cout<<"tax amount"<<tax;
    }
     else if (amt>50000&& amt<=100000){
       tax=amt*20/100;
        cout<<"tax amount"<<tax;
    }
     else if (amt>100000&& amt<=200000){
       tax=amt*10/100;
        cout<<"tax amount"<<tax;
    }
    else {
       tax=amt*40/100;
        cout<<"tax amount"<<tax;
    }
}

4.Nested if

= if condition 
{
//statement;

if condition 
{
//statement;
}

 else 
{
//statement;
}
}

else 
{
//statement;
}
