# codewithvaibhav
#include<iostream>
#include<stdlib.h>
#include<time.h>
using namespace std;

int main() {
    int num,guess,nguesses{1};
    srand(time(0));
    num=rand()%100+1;
    do{
        cout<<"guess the number btw 1-100"<<endl;
        cin>>guess;
        if(guess>num){
            cout<<"lower number please !"<<endl;

        }
        else if(guess<num){
            cout<<"higher number please !"<<endl;
        }
        else{

            cout<<"yeah you guessed the number "<<nguesses<<endl;
        }
        nguesses++;
    }
    while(guess!=num);

return 0;
}
