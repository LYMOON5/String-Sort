
//字符串不等长
void StrSort(char *str[10])
{
	char tmp[100];
	char *str = (char *)malloc(10*sizeof(char));
	for(int i = 0;i < 10;i++)
	{
		for(int j = 0;j < 10-i;j++)
		{
			if(strcmp(str[j],str[j+1])>0)
			{
				strcpy(tmp,str[j]);
				strcpy(str[j],str[j+1]);
				strcpy(str[j+1],tmp);
			}
		}
	}
}

