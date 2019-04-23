/*
 * @Date: 2019-4-23
 * @Author: tracycw
 * @Description: 计数排序
 */

#define _CRT_SECURE_NO_WARNINGS
#include <iostream>
#include <algorithm>

using namespace std;

void get_max_min(int a[], int*& max, int*& min, int len)
{
	max = max_element(a, a + len);
	min = min_element(a, a + len);
}

int main()
{
	int a[] = {92, 91, 95, 90, 99, 91, 97, 94, 92, 99};
	int len = sizeof(a) / sizeof(a[0]);
	
	int* max = NULL;
	int* min = NULL;

	get_max_min(a, max, min, len);

	int size = *max - *min + 1;
	int* ret = new int[size];
	memset(ret, 0, sizeof(int)*size);

	for (int i = 0; i < len; ++i)
	{
		ret[a[i] - *min]++;
	}

	for (int i = 0; i < len; ++i)
	{
		for (int j = 0; j < ret[i]; ++j)
		{
			cout << *min + i << " ";
		}
	}
	cout << endl;

	system("pause");
	return 0;	
}
