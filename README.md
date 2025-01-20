# firstdemo Ticket Priceing
this is my first demo repository
<br>
Auther - Dhyan chandra Ravi
<br>
#include<iostream>
using namespace std;
int main (){
    int age;
    cout<<"enter age :";
    cin>>age;

    if(age>=0 && age<=100){
        cout<<"valid age"<<endl;
    }
    int ticketprice;
    if(age<=5){
        ticketprice=0;
    }
    else if(age>5 && age<=18){
        ticketprice=100;
    }
    else if(age>18 && age<=60){
        ticketprice=200;
    }
    else{
    ticketprice=150;
    }
    cout<<"Ticket price : "<<ticketprice<<endl;

    int type;
    cout<<"Enter Ticket Type : "<<endl;
    cout<<"1-normal, 2-dilux, 3-premium"<<endl;
    cin>>type;

    if(type==2){
        ticketprice+=50;
    }
    else if(type==3){
        ticketprice+=100;
    }
    string discount;
    cout<<"do you want discount coupon"<<endl;
    cin>>discount;
    if(discount=="yes"){
        ticketprice = 0.9*ticketprice;
    }
    cout<<"Final Price : "<<ticketprice<<endl;
    return 0;
}
