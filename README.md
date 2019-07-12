# C 언어    겁나 어려움 뭐라는지 1도 모르겠음


C+

최대 최초값

void main()
{
      int max, i, min:++
      max = -999;
      min = 999:
      for (i = 0: i < 10: i++)
      {
                  if (max < d[ i ])
                     max =d[ i ]:
                  if (min > d[ i ])
                     min = d[ i ]:
      }
      printf("10개중 최대값은 %d, 최소값은 %d 입니다.",max, min
}





********************************************************************************************

void main()
{
      int max, i, min:
      int d[ ] = { -7,-3,-2,-9,-5,-8,-4,-6,-11,-1 }:
      max = d[0]:
      min = d[0]:
      for ( i = 1: i < 10: i++)
      {
                  if (max < d[ i ])
                     max =d[ i ]:
                  if (min > d[ i ])
                     min = d[ i ]:
      }
      printf("10개중 최대값은 %d, 최소값은 %d 입니다.",max, min:
}



********************************************************************************************

#include <stdio.h>
void main()
{
	int dan = 7, i, x;
	for (i = 1 ; i <= 9 ; i++)
	{
		x = dan * i;

		printf("%d * %d = %2d \n",dan ,i,x);
	}




********************************************************************************************
구구단

#include <stdio.h>

 void main()
{
 int i, j, x;

 for (i = 2; i <= 9; i++)
 {
  printf("=========%d단=========\n", i);
   for (j = 1; j <= 9; j++) {
     x= i * j;
   printf("%d * %d =%d \n",i,j,x);

  }

 }
}


********************************************************************************************
구구단 정리

#include <stdio.h>

void main()
{
	int i, j, x;
	for (i = 2; i <= 9; i++)
	{
		printf("=========", i);
	}
	printf("\n");
		for (i = 2; i <= 9; i++)
	{
		printf("=구구 %d단=", i);
	}
	printf("\n");
	for (i = 2; i <= 9; i++)
	{
		printf("========");
	}
	printf("\n");
	for (i = 1; i <= 9; i++)
	{
		for (j = 2; j <= 9; j++)
		{
			x = j * i;
			printf("%d * %d = %2d ", j, i, x);
		}
		printf("\n");
	}
	for (i = 2; i <= 9; i++)
	{
		printf("==========");
	}
	printf("\n");
}



********************************************************************************************

??

#include <stdio.h>
void main()
{
	int i, s =0;
	for (i = 1; i <= 100; i++)
		s += i;
	printf("*1+2+3+,,,,+100=%d\n", s);
}



********************************************************************************************

홀 짝


#include <stdio.h>
void main()
{
	int i, s1=0, s2=0;
	for (i = 1; i <= 100; i+=2)
	{
		s1 += i;

		printf("%d+", i);
		if (i == 99) printf("=");
		else printf("+");
	}
	printf("홀수합=%d\n", s1);
	for (i = 2; i <= 100; i += 2)
	{
		s2 += i;

		printf("%d+", i);
		if (i == 100) printf("=");
		else printf("+");
	}
printf("짝수함=%d\n", s2);
}




********************************************************************************************


홀 짝  간단하게 
C언어는 


#include <stdio.h>
void main()
{
	int i, s1=0, s2=0;
	for (i = 1; i <= 100; i++)
	{
		if (i % 2)
			s1 += i;
		else 
			s2 += i;
	}
	printf("홀수합=%d\n", s1);
	printf("짝수함=%d\n", s2);
}





********************************************************************************************




#include <stdio.h>
void main()
{
	int i, s1 = 0, s2 = 0, sw = 1;
	/*
	// 2로 나눈 나머지 홀 짝 구별
	for (i = 1; i <= 100; i++)
	{
		if (i % 2)
			s1 += i;
		else
			s2 += i;
	}
	// swirch 법
	for (i = 1; i <= 100; i++)
	{
		if (sw)
		{
			s1 += i;
			sw = 0;
		}
		else
		{
			s2 += i;
			sw = 1;
		}
	}
	*/
	// 50회전 방법
	for (i = 1; i <= 100; i+=2)
	{
			s1 += i;
			s2 += i+1;
	}
	printf("홀수합=%d\n", s1);
	printf("짝수함=%d\n", s2);
}


**********************************************************************

다이아몬드

#include <stdio.h>
int main()
{
	int column = 5;
	int row = column;
	
	for (int i = 1; i <= column; i++)
	{
		for (int j = row - i; j > 0; j--)
		{
			printf("0");
		}
		for (int k = 0; k < i; k++)
		{
			printf("*");
		}
		for (int k = 0; k < i-1; k++)
		{
			printf("*");
		}
		for (int j = (row - i); j > 0; j--)
		{
			printf("0");
		}
		printf("\n");
	}
	for (int i=1;i <= column-1;i++)
	{
		for (int j = 0; j < i; j++)
		{
			printf("0");
		}
		for (int k = (row - i); k > 1; k--)
		{
			printf("*");
		}
		for (int k = i; k < row; k++)
		{
			printf("*");
		}
		for (int j = 0; j < i; j++)
		{
			printf("0");
		}
		printf("\n");
	}
	
}



********************************************************************
