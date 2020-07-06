# Function_Overloading-C++-
Performing the type of POLYMORPHISM which make us understand the principle of Early Binding also by matching the arguments of the functions having same name but performing different jobs which we call in all Function Overloading.Here function name is area common name for both the functions but performing different jobs by calculating the area for different shapes rectangle and circle.

#include<iostream>
#include<conio.h>
using namespace std;
int area(int,int);
float area(int);
int main()
{
	int l,b,m,r;
	float k;
	cout<<"enter the length & breadth of rectangle:";
	cin>>l>>b;
	m = area(l,b);
	cout<<"area of rectangle = "<<m<<endl;
	cout<<"enter the radius of the circle";
	cin>>r;
	k = area(r);
	cout<<"area of circle ="<<k;
	return 0;
}
int area(int x,int y)
{
	return(x*y);
}
float area(int z)
{
	return(3.14*z*z);
}
