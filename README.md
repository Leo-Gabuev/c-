# c-
Дано четырехзначное число (к примеру 5678), вывести на экран  в обратном порядке цифры из которых это число состоит. То есть мы должны увидеть на экране 8765. Подсказка: чтобы взять из числа отдельные цифры, надо применять  деление по модулю на 10.
#include <iostream>
using namespace std;
int main()
{
	setlocale(LC_ALL, "ru");
	int a;
	cout << "введите четырехзначное число";
	cin >> a;
	cout << a % 10;
	a /= 10;
	cout << a % 10;
	a /= 10;
	cout << a % 10;
	a /= 10;
	cout << a % 10;
	a /= 10;
	cout << endl;
}
  
  
  
  
