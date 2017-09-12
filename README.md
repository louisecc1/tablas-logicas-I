#include<iostream>
using namespace std;
int main(){
  int b,c,d;
  string a;
  a="a2(1)21";
  bool e=true;
  c=0;
  while (e)
  {
    for(b=1;b<a.size();++b){
      if(a[c]=='('){
        if(a[b]!=')'){
          e=false;
        }
      }
    }
    if(c==16){
      e=true;
      break;
    }
    ++c;
  }
  cout<<e<<"\n";
  return 0;
}
