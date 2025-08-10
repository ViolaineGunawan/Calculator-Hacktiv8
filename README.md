# Calculator-Hacktiv8
Capstone Project from Hacktiv8

#include <bits/stdc++.h>
using namespace std;

int main() {
	for (;;) {
		string a = "", b = "", c = "";
		int aa = -1, bb = -1;
		while (aa == -1) {
			char angka;
			cin >> angka;
			switch (angka) {
				case '1':
					a += '1';
					break;
				case '2':
					a += '2';
					break;
				case '3':
					a += '3';
					break;
				case '4':
					a += '4';
					break;
				case '5':
					a += '5';
					break;
				case '6':
					a += '6';
					break;
				case '7':
					a += '7';
					break;
				case '8':
					a += '8';
					break;
				case '9':
					a += '9';
					break;
				case '0':
					a += '0';
					break;
				default:
					aa = 0;
					c += angka;
			}
		}
		while (bb == -1) {
			char ang;
			cin >> ang;
			switch (ang) {
				case '1':
					b += '1';
					break;
				case '2':
					b += '2';
					break;
				case '3':
					b += '3';
					break;
				case '4':
					b += '4';
					break;
				case '5':
					b += '5';
					break;
				case '6':
					b += '6';
					break;
				case '7':
					b += '7';
					break;
				case '8':
					b += '8';
					break;
				case '9':
					b += '9';
					break;
				case '0':
					b += '0';
					break;
				default:
					bb = 0;

			}
		}
		int x = stoi(a), y = stoi(b);
		if (c[0] == '+') {
			cout << x + y;
		} else if (c[0] == '-') {
			cout << x - y;
		} else if (c[0] == '/') {
			double d = x / (y * 1.0);
			cout << fixed << setprecision(5) << d;
		} else if (c[0] == '*') {
			cout << x *y;
		}

	}
	return 0;
}
