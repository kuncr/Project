#include<iostream>
#include<math.h>
using namespace std;
int giaiPT(float a, float b, float &x) {
    if (a == 0) {
        if (b == 0)
            return 2;
        return 0;
    }
    x = -b / a;
    return 1;
}
int main() {
    float a, b,x;
    cout << "Nhap a:";
    cin >> a;
    cout << "Nhap b:";
    cin >> b;
    if (giaiPT(a, b, x) == 0)
        cout << "Phuong trinh vo nghiem"<<endl;
    else if( giaiPT(a,b,x) == 1)
        cout << "Phuong trinh co mot nghiem: " <<x<< endl;
    else
        cout << "Phuong trinh co vo so nghiem" << endl;
    return 0;
}
