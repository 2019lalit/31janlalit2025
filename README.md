Que:-  Write a program to multiply all the digits of a number until the result is a single digit.
       input:-  39
       Result: 4

Answer:--
          
          #include<bits/stdc++.h>
using namespace std;
int Multiplydigit(int num){
    int product;
    while(num>=10){
         product=1;
         while(num>0){
            
             product=product*(num%10);
             num=num/10;
         } num = product;
    } return num;
}
int main(){
    int num;
    cout<<"please enter a number"<<endl;
    cin>>num;
    int result=Multiplydigit(num);
    cout<<"the single digit is "<<result;
    return 0;
}

-------------------------------------------------------------------------------------------------------------------------
Write a program to multiply all the digits of a number
input : 781
output: 56


   #include<bits/stdc++.h>
using namespace std;
int Multiplydigit(int num){
  
        int product=1;
        while(num>0){
          product=product * (num%10);
          num=num/10;
            
        } return product;
        
        
}
  
int main(){
    int num;
    cout<<"please enter a number"<<endl;
    cin>>num;
   cout<< Multiplydigit(num);
   
}

---------------------------------------------------------------------------------------------------------------------
Write a program to sum all the digits of a number
781
output: 16

   #include<bits/stdc++.h>
using namespace std;
int Sumdigit(int num){
  
        int product=0;
        while(num>0){
          product=product + (num%10);
          num=num/10;
            
        } return product;
        
        
}
  
int main(){
    int num;
    cout<<"please enter a number"<<endl;
    cin>>num;
   cout<< Sumdigit(num);
   
}

-----------------------------------------------------------------------------------------------------------------------------
Write a program to count all the digits of a number
781
output: 3

   #include<bits/stdc++.h>
using namespace std;
int countdigit(int num){
    if(num==0){
        return 1;
    }
      int count=0;
      while(num>0){
          count++;
          num=num/10;
      }
      return count;
    
}
  
int main(){
    int num;
    cout<<"please enter a number"<<endl;
    cin>>num;
   cout<< countdigit(num);
   
}

-------------------------------------------------------------------------------------------------------------
largest number of given digit



   #include<bits/stdc++.h>
using namespace std;
int largestdigit(int num){
int largest=0;
while(num>0){
    int digit=num%10;
    if(digit>largest){
        largest=digit;
    } num=num/10;
}
    return largest;
}
  
int main(){
    int num;
    cout<<"please enter a number"<<endl;
    cin>>num;
   cout<< largestdigit(num);
   
}


------------------------------------------------------------------------------------------------------------------------------------------------


