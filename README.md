#include<iostream>
#include<cstdlib>
#include<ctime>
using namespace std;
int main()
{
	srand((unsigned int)time(NULL));//random integers to generated by using time because by every diff time diff integer is generated
	int number= (rand()%100)+1; //because we need integers in the range 1-100 and rand will generate from 0 to higher number
	int guess=0;
	do{
		cout<<"Guess any number between 1-100:";
		cin>>guess;
		if(guess>number)
		 cout<<"Guess any lower number!"<<endl;
		else if(guess<number)
		 cout<<"Guess any higher number!"<<endl;
		else
		cout<<"You Won!!Congratulations..."<<endl;
	}while(guess!=number);
	return 0;
}
