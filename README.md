# randumnumm
#include<iostream>
#include <cstdlib>
#include <ctime>
using namespace std ;
int main (){
    int num , randnum,i;
     cout << " ---------- TRUST YOUR GUTS ----------"<<endl;
     cout << "  You'll be given 5 attempts to guess the secretnumber from 1 to 100 "<<endl;
     cout << " Let's get started...."<<endl;
     srand(time(0));
      randnum = 1 + (rand() %100);
for( i = 1 ; i <=5 ;i++){
     cout <<  " Enter your number :"<<endl;
     cin>>num;
     if (num== randnum){
        cout<<" you got it !!"<<endl;
        cout<<" press enter to replay"<<endl;
        break;
     }
     else if(num >randnum) {
        cout<<"our secret number is smaller "<<endl;
     }
     else{
        cout<<"our secret number is greater "<<endl;
     }
if(i==5){
    cout<<"oops you can't guessed it ,the secretnumber was : "  <<randnum<<endl;
   
}
}
 cout<<" Press enter to replay "<<endl;
cin.ignore();
cin.get();
return 0;

}
