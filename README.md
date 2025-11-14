\\# multi-level-inheritance
\\this code only use to tourbo cpp



 #include<iostream>
#include<conio.h>
using namespace std;
class student

{

protected:

int roll;

public:



void get_roll(int m);
roll=m;
void display_roll()
{
cout<<"\n roll="<<roll;
}
};
class marks: public student {

protected:

int m1, m2;

public:

void get_mark(int p, int q)
{
m1=p;
m2=q;
}

void display_mark()

{

cout<<"\n markks != "<< m1;

cout<<" \n marks2="<<m2;

}
};

class final:public marks
{
int total;

public:

void display()
{
total=m1+m2;

display_roll();

display_mark();

Cout<<"\n total="<<total;
}
};


int main()
{
find obj;

obj.get_roll(1001);

obj.get_mark(50,80);

obj.display();

getch();
}
