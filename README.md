#include<iostream>
using namespace std;
int main()
{
	int a[10][10], j , i ,h, k = 1;
	for (int i = 0; i <= 9; i++)
		for (int j = 0; j <= 9; j++)
		{
			a[i][j] = k;
			k++;
			cout << a[i][j] << " ";

			if (j == 9)
				cout << endl;
		}
	for (int i = 0; i <= 9; i++)
		for (int j = 0; j <= 9; j++)
		{
			h = i * 10 + j;
			for (int x = 2; x < h; x++)
				if (h % x != 0)
					cout << a[i][j] << " ";
					
		}
		
	return 0;
}
