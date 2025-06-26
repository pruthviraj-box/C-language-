# C++-language-
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

