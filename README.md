# -function-that-returns-multiple-results-using-reference-parameters.

#include<iostream>
  using namespace std;
   void result(int a,int b,int &sum,int &diff, int &multiple , int &divide){
       sum=a+b;
       diff=a-b;
       multiple=a*b;
       if(b!=0){
           divide=a/b;
       }
       else
       cout<<"divide does not possible";
   }
    int main(){
     int a,b,sum , diff , multiple, divide ;
     cout<<"enter the value of two numbers : ";
     cin>>a>>b;
     
     result(a,b,sum , diff , multiple, divide);
     
     cout<<"addition of two number"<<sum<<"\n";
     cout<<"subtraction of two numbers"<<diff<<"\n";
     cout<<"multiplication of two numbers"<<multiple<<"\n";
     cout<<"division of two numbers"<<divide<<"\n";
     
     return 0;
    }
