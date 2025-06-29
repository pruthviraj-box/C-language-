hi# C++-language-
Program language oops

class= class is the user defined data type or blue print that wrapped data and functions in to the single entity.

syntax= class classname{
                    data
                      +
                  function};
                  
object= object is a contract representation of the blue print that is defined by the class.

Ex #include <iostream>


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

Features of oops
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


TOKENS 

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
     rules to 

