# Leibniz-formula-for-pi
循环，不断加减（引入sign）来实现
#include <iostream>
using namespace std;
int main() {

	double pi = 0;
	double a;
	int n = 1;
	int sign = 1;
	while (abs(1.0 / n) >= 1e-6)
	{
		a = 1.0 / n*sign;
		
		pi = pi + a;
		n = n+2;
		sign = -sign;
		
		



	}
	pi = pi * 4;

	cout << "pi=" << pi << endl;

