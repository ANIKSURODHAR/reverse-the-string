# reverse-the-string


//cod here


#include <bits/stdc++.h>

using namespace std;

int main() {
    
  int t;
  cin>>t;
  cin.ignore();
 while(t--){
       
 string str;
 
 getline(cin,str);
 
 string word="";

 for(int i=0;i<str.size();i++){
     
     if(str[i]==' '){
         
         reverse(word.begin(),word.end());
         
         cout<<word;
         
         word="";
         cout<<' ';
     }
     else{
         
         word+=str[i];
         
     }
 }
 
 reverse(word.begin(),word.end());
         
 cout<<word;
 
 cout<<"\n";
 

 }

    return 0;
}
