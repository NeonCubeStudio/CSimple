### If else statements
Application.csimple
```
include System;		/* print function */

public static int32 Main(void)
{
	unsigned int8 cookies = 3;
	
	if (cookies == 0)
	{
		Print("We have no cookies!");
	}
	else if (cookies == 1)
	{
		Print("We have 1 cookie!");
	}
	else
	{
		Print("We have 2 or more cookies!");
	}

	return 0;
}
```