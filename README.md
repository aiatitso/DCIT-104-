# DCIT-104-

#include <iostream>
using namespace std;
 void prime(int x);
int main()
{
int p = 0;

    cout << "Any number : " <<endl;
    cin >> p ;
    prime(p);
    
}
 void prime (int x)
 {
   int sum = 0;
    for (int f = x ; f > 1  ; f--)
    {

    bool isPrime = true;
    for (int j = 2 ; j < f ; j++)
    {
        if(f % j == 0)
            {
            isPrime = false;
            j = f;
            }
    }
    if (isPrime == true)
        {
        cout << "prime number: " << f << " , " ;
        sum = sum + f;
        }
    }
    cout << endl<< "sum of the given prime numbers : " << sum ;



}
