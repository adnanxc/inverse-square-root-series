# inverse-square-root-series

#include <iostream>
#include <cmath>
using namespace std;

void series(int n){
    cout << "1 ";

    for(int c=2; c<=n; c++){
        cout << "+ (1/(" << c << ")^0.5) ";

    }

    cout << "= ";
    float sum = 0;

    for(int i=1; i<=n; i++){
        sum = sum + (1/sqrt(i));
    }
    cout << sum;
}

int main(){

    int x;
    cout << "Enter an integer: ";
    cin >> x;
    series(x);

    return 0;
}
