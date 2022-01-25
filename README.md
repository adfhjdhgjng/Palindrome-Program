// Palindrome-Program
#include<iostream.h>
int main()
{
  int n, num, digit, rev= 0;
  cout<<"\n Input the number (max. 32767):";
  cin>> num;
  n=num;
  do
{
   digit= num%10; 
   rev=(rev*10)+digit;
   num=num/10;
}
   while(num!=0);
cout<<"The reverse of the number is:"<<rev<<"\n";
if(n==rev)
  cout<<"The number is palindrome";
else
  cout<<"\n The number is not a palindrome";
return 0;
}
