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
  
  Пользователь вводит порядковый номер пальца руки. Необходимо показать его название на экран.
  
  #include <iostream>
using namespace std;
int main()
{
	setlocale(LC_ALL, "ru");
	int a;
	cout << "введите цифру";
	cin >> a;
	if (a == 1)
		cout << "большой палец";
	else if (a == 2)
		cout << "указательный палец";
	else if (a == 3)
		cout << "fuck";
	else if (a == 4)
		cout << "безымянный";
	else if (a == 5)
		cout << "мезинец";
	cout << endl;
}

Еще одна задача для самостоятельно решения.  Необходимо написать программу, которая проверяет пользователя на знание таблицы умножения. Пользователь сам вводит два целых однозначных числа. Программа задаёт вопрос: результат умножения первого числа на второе.  Пользователь должен ввести ответ и увидеть на экране правильно он ответил или нет. Если нет  – показать еще и правильный результат.

#include <iostream>
using namespace std;
int main()
{
	setlocale(LC_ALL, "ru");
	int a, b,c;
	cout << "введите первую цифру";
	cin >> a;
	cout << "введите вторую цифру";
	cin >> b;
	cout << "перемножить числа";
	cin >> c;
	if (c == a*b)
		cout << "верно";
	else 
		cout << "неверно"<<a*b;
	cout << endl;
}
Составить расписание на неделю. Пользователь вводит порядковый номер дня недели и у него на экране отображается, то, что запланировано на этот день.

#include <iostream>
using namespace std;
int main()
{
	setlocale(LC_ALL, "ru");
	int a;
	cout << "введите день недели ";
	cin >> a;
	switch (a)
	{
	case 1:
		cout << "пойти в зал\n";
		cout << "забрать детей";
	case 2:
		cout << "выучить стих\n";
		cout << "написать программу";
		//и так далее
		break;
	default:
		cout << "нет такого дня";
	}
	
		cout << endl;
}



#include <iostream>
using namespace std;
int main()
{
	double n;
	int summ_n = 0;
	cout << "enter number";
	cin >> n;
	if ((n - int(n)) != 0)
	{
		cout << "n is wrong";
	}
	else
	{
		for (int i = 1; i < n + 1; i++)
		{
			summ_n += i;
		}
		cout << "summ_n=" << summ_n << endl;
		return 0;
	}
}
