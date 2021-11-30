# cplus2.0_switchcase-
selling products using switch case

#include <iostream>
using namespace std;

int main()
{
     int number, n;
     int total=0;
     int cash;
     char ask;
     int price [5]={6550,7845,950,1350,970};
     
     retry:
     
     cout<<"=========================================="<<endl;
     cout<<"| GROUP#2 GOLDEN WARRIORS(PROGRAMMERS)   |"<<endl;
     cout<<"|========================================|"<<endl;
     cout<<"| WIDE MIND TECHONOLOGY COMPUTER SHOP    |"<<endl;
     cout<<"|========================================|"<<endl;
     cout<<"|                 LIST                   |"<<endl;
     cout<<"|========================================|"<<endl;
     cout<<"|  NAME OF PRODUCTS   \t ||     PRICE    |"<<endl;
     cout<<"|1. VERTICAL MONITOR  \t || Php.7556     |"<<endl;
     cout<<"|2. CPU               \t || Php.7994     |"<<endl;  
     cout<<"|3. WIRELESS KEYBOARD \t || Php.890      |"<<endl;
     cout<<"|4. WIRELESS MOUSE    \t || Php.875      |"<<endl;
     cout<<"|5. HEADPHONE         \t || Php.875      |"<<endl;
     cout<<"|========================================|"<<endl;
     
     cout<<" Enter a number of a product that you wish to buy: ";
     cin>>number;
     
     switch (number){
          case 1:
          cout<<" Enter how many you want to buy:";
          cin>>n;
          
          total +=price [0]*n;
          cout<<" Do you want to buy more? (y/n) ";
          cin>> ask;  
          
          if (ask =='y'){
              goto retry;
          }else
              goto end;
              
          case 2:
          cout<<" Enter how many you want to buy: ";
          cin>>n;
          
          total+=price [1]*n;
          cout<<" Do you want to buy more? (y/n): ";
          cin>>ask;
          
          if (ask =='y'){
              goto retry;
          }else
              goto end;
              
          case 3:
          cout<<" Enter how many you want to buy: ";
          cin>>n;
          
          total+=price [2]*n;
          cout<<" Do you want to buy more? (y/n): ";
          cin>>ask;
          
          if (ask =='y'){
              goto retry;
          }else
              goto end;   
            
          case 4:
           cout<<" Enter how many you want to buy: ";
          cin>>n;
          
          total+=price [3]*n;
          cout<<" Do you want to buy more? (y/n): ";
          cin>>ask;
          
          if (ask =='y'){
              goto retry;
          }else
              goto end;
          
          case 5:
          cout<<" Enter how many you want to buy: ";
          cin>>n;
          
          total+=price [4]*n;
          cout<<" Do you want to buy more? (y/n): ";
          cin>>ask;
          
          if (ask =='y'){
              goto retry;
          }else
              goto end;  
     }
     end:
        cout<<" Total price you must pay is =php." <<total<<"\n";
        cout<<" Cash: ";
        cin>>cash;  
        
            cout<<" Change: "<< cash-total<<"\n\n";
            cout<<" Thank for purschasing our products "<<"\n\n";
            
return 0;
}
            
  /*output:
  
  ==========================================
| GROUP#2 GOLDEN WARRIORS(PROGRAMMERS)   |
|========================================|
| WIDE MIND TECHONOLOGY COMPUTER SHOP    |
|========================================|
|                 LIST                   |
|========================================|
|  NAME OF PRODUCTS   	 ||     PRICE    |
|1. VERTICAL MONITOR  	 || Php.7556     |
|2. CPU               	 || Php.7994     |
|3. WIRELESS KEYBOARD 	 || Php.890      |
|4. WIRELESS MOUSE    	 || Php.875      |
|5. HEADPHONE         	 || Php.875      |
|========================================|
 Enter a number of a product that you wish to buy: 2
 Enter how many you want to buy: 3
 Do you want to buy more? (y/n): n
 Total price you must pay is =php.23535
 Cash: 5000
 Change: -18535

 Thank for purschasing our products.  */  
