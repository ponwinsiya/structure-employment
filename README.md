#include <iostream>
using namespace std;
  
struct employee {
    string ename;
    int age, phn_no;
    int salary;
};
  
// Function to display details of all employees
void display(struct employee emp[], int n)
{
    cout << "Name\tAge\tPhone Number\tSalary\n";
    for (int i = 0; i < n; i++) {
        cout << emp[i].ename << "\t" << emp[i].age << "\t"
             << emp[i].phn_no << "\t" << emp[i].salary << "\n";
    }
}
  
// Driver code
int main()
{
    int n = 3;
    // Array of structure objects
    struct employee emp[n];
  
    // Details of employee 1
    emp[0].ename = "Winsi";
    emp[0].age = 23;
    emp[0].phn_no = 256785490;
    emp[0].salary = 40000;
  
    // Details of employee 2
    emp[1].ename = "Reenu";
    emp[1].age = 30;
    emp[1].phn_no = 987643210;
    emp[1].salary = 56000;
  
    // Details of employee 3
    emp[2].ename = "Smile";
    emp[2].age = 43;
    emp[2].phn_no = 654189098;
    emp[2].salary = 60500;
  
    display(emp, n);
  
    return 0;
}
