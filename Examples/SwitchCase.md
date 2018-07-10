### Switch case
Application.csimple
```
include System;		/* print function */

public enum CookieTypes
{
	ZaansHuisje = 0,
	Deugnietje,
	Biscuit,
}

public static int32 Main(void)
{
	CookieTypes cookie = CookieTypes.ZaansHuisje;
	
	switch (cookie)
	{
		case (CookieTypes.ZaansHuisje || CookieTypes.ZaansHuisje)
		{
			Print("It's a special cookie!");
			
			break;
		}

		case (CookieTypes.Biscuit)
		{
			Print("It's a biscuit!");

			break;
		}

		default
		{
			Print("It's a mysterious cookie!");

			break;
		}
	}

	return 0;
}
```