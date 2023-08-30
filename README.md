// NUMBER GUSSING GAME..................................
#include<iostream>
#include<cstdlib>
#include<ctime>
using namespace std; 
int main()
{
	int num,guess;
	srand(time(0));
	num=rand()%100+1;
	do
	{
		cout<<"Enter a guess between 1 and 100:";
		cin>>guess;

		if(guess>num)
			cout<<"Guess is too high!\n\n";
		else if(guess < num)
			cout<<"Guess is too low!\n\n";
		else
			cout<<"\nCorrect Guess!\n",num;
	} while(guess!=num);

	return 0;
}
