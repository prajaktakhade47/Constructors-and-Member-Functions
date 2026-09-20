#include <iostream>
#include <string>
using namespace std;

class Student{
private:
    int rollNo;
    string name;
    float marks;
public:
    //Default Constructor
    Student(){
        rollNo = 0;
        name = "Not Set";
        marks = 0.0;
        cout << "\nDefault Constructor called: Object created with default values." << endl;
    }
    //Parameterized Constructor
    Student(int r, string n, float m){
        rollNo = r;
        name = n;
        marks = m;
        cout << "\nParameterized Constructor called: Object created with given values." << endl;
    }
    //Copy Constructor
    Student(const Student &s){
        rollNo = s.rollNo;
        name = s.name;
        marks = s.marks;
        cout << "\nCopy Constructor called: Object copied from another object." << endl;
    }
    void setMarks(float m){
        marks = m;
        cout << "Marks updated using inside-class member function." << endl;
    }
    void displayData();

    // Destructor
    ~Student(){
        cout << "Destructor called: Object with Roll No " << rollNo << " destroyed." << endl;
    }
};
void Student::displayData(){
    cout <<"Roll No : "<<rollNo<<endl;
    cout<<"Name    : "<<name<<endl;
    cout<<"Marks   : "<<marks<<endl;
}
int main(){
    cout<<"========================================="<<endl;
    cout<<" DEMONSTRATION OF TYPES OF CONSTRUCTORS "<<endl;
    cout<<"========================================="<<endl;

    // Calling Default Constructor
    cout<<"\n--- Default Constructor Demo ---"<<endl;
    Student s1;
    s1.displayData();

    cout << "\n--- Parameterized Constructor Demo ---" << endl;
    Student s2(101, "Prajakta Khade", 89.5);
    s2.displayData();

    cout << "\n--- Copy Constructor Demo ---" << endl;
    Student s3(s2);
    s3.displayData();
    
    cout << "\n--- Member Function Defined Inside Class ---" << endl;
    s1.setMarks(75.0);
    s1.displayData();

    cout << "\n--- Member Function Defined Outside Class ---" << endl;
    s2.displayData();
    cout << "\n=========================================" << endl;
    cout << " END OF PROGRAM - DESTRUCTORS WILL NOW RUN " << endl;
    cout << "=========================================" << endl;

    return 0;
}
