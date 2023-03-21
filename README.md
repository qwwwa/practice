/*
编写代码，演示多个字符移动，向中间汇聚
welcome to there!!!
w#################!
we###############!!
wel#############!!!
…
welcome to there!!!
*/

#include<stdio.h>
#include<windows.h>
int main()
{
	char arr1[] = "welcome to there!!!";
	char arr2[] = "###################";
	int left = 0;
	int right = strlen(arr1)-1;

	while (left<=right)
	{
		arr2[left] = arr1[left];
		arr2[right] = arr1[right];

		printf("%s\n", arr2);
		Sleep(1000);	//睡眠一秒
		system("cls");	//清空屏幕

		left++;
		right--;

	}
	printf("%s\n", arr2);
	return 0;
}
