#include<iostream>
using namespace std;
void input(int &a, int &b, int &c, int &d, int &e, int &f)
{
    cout<<"Enter number of pennies:";
    cin>>a;
    cout<<"\nEnter number of nickels:";  
    cin>>b;
    cout<<"\nEnter number of dimes:"; 
    cin>>c;
    cout<<"\nEnter number of quarter:";   
    cin>>d;
    cout<<"\nEnter number of half dollars:";  
    cin>>e;
    cout<<"\nEnter number of dollars:";
    cin>>f;
}
int pennies(int a)
{
    return a*1;
}
int nickels(int b)
{
    return b*5;
}
int dimes(int c)
{
    return c*10;
}
int quarter(int d)
{
    return d*25;
}
int halfdollars(int e)
{
    return e*50;
}
int dollars(int f)
{
    return f*100;
}
int calculate(int a, int b, int c, int d, int e, int f)
{
   int sum;
   sum=pennies(a)+nickels(b)+dimes(c)+quarter(d)+halfdollars(e)+dollars(f);
   return sum;
}
int main()
{
    int a,b,c,d,e,f;
    input(a,b,c,d,e,f);
    int sum=calculate(a,b,c,d,e,f);
    cout<<"\nYou have"<<" "<<a<<" "<<"pennies"<<endl;
    cout<<"You have"<<" "<<b<<" "<<"nickels"<<endl;
    cout<<"You have"<<" "<<c<<" "<<"dimes"<<endl;
    cout<<"You have"<<" "<<d<<" "<<"quarters"<<endl;
    cout<<"You have"<<" "<<e<<" "<<"half dollars"<<endl;
    cout<<"You have"<<" "<<f<<" "<<"dollars"<<endl;
    cout<<"You have"<<" "<<sum<<" "<<"cent"<<endl;
    return 0;
}
