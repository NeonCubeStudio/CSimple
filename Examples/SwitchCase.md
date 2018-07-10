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
			print("It's a special cookie!");
		}

		case (CookieTypes.Biscuit)
		{
			print("It's a biscuit!");
		}

		default
		{
			print("It's a mysterious cookie!");
		}
	}

	return 0;
}
```