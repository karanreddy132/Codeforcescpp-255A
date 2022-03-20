# Codeforcescpp-255A
#include <bits/stdc++.h>
 
using namespace std;
 
int main(){
  int n,chest(0),biceps(0),back(0),ele;
  cin >> n;
  for(int i=0;i<n;i++){
    cin >> ele;
    if((i%3)==0)
      chest+=ele;   
    else if((i%3)==1)
      biceps+=ele;
    else
      back+=ele;
  }
  if(chest > biceps && chest > back)
    cout << "chest";
  else if(biceps > chest && biceps > back)
    cout << "biceps";
  else
    cout << "back";
  return 0;
}
