# c-string-using-str-compare-fun
#include <stdio.h>
#include<string.h>
#define MAX_SIZE 100
int main()
{
  char str1[MAX_SIZE], str2[MAX_SIZE];
  int res;
  printf("enter first string:");
  scanf("%s",str1);
  printf("enter second sring:");
  scanf("%s",str2);
  res = strcmp(str1, str2);
  if(res == 0)
  {
    printf("both strings are equal.");
  }
  else if(res == -1)
  {
    printf("first string is lexicographically smaller than second. ");
  }
  else
  {
    printf("first string is lexicographically greater than second.");
  }
  return 0;
}
