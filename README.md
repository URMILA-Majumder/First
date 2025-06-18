# First
#include <bits/stdc++.h>

using namespace std;
class student
{
public:
    int id;
    char name[100];
    char sec[100];
    int marks;

};



int main()
{
    int t;
    cin >> t;
    while(t--)
    {
        student a,b,c;
        cin.getline(a.name,100);
        cin >>a.id >> a.name  >> a.sec >> a.marks;

        cin.getline(b.name,100);
        cin >>b.id >> b.name  >> b.sec >> b.marks;

        cin.getline(c.name,100);
        cin >>c.id >> c.name  >> c.sec >> c.marks;
        if(a.marks > b.marks && a.marks > c.marks)
        {
            cout << a.id << " " << a.name << " " << a.sec << " " << a.marks << endl;
        }
        else if(b.marks > a.marks && b.marks > c.marks)
        {
            cout << b.id << " " << b.name << " " << b.sec << " " << b.marks << endl;
        }
        else if(c.marks > a.marks && c.marks > b.marks)
        {
            cout << c.id << " " << c.name << " " << c.sec << " " << c.marks << endl;
        }
        else if(c.marks > a.marks && c.marks > b.marks)
        {
            cout << c.id << " " << c.name << " " << c.sec << " " << c.marks << endl;
        }
        else if(a.marks == b.marks || c.marks == b.marks || c.marks == a.marks)
        {
            cout << a.id << " " << a.name << " " << a.sec << " " << a.marks << endl;
        }


    }


    return 0;
}
