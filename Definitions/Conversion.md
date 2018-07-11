### Conversion
It is possible to convert ```float(x)```, ```int(x)```, ```enum``` to each other

Example (int32 and float32 to float64)
```
public static int32 Main(void)
{
	int32 a = 1;
	float32 b = 2.0;
	float64 c = (float64)a + (float64)b;

	return 0;
}
```

Example (int32 and float32 to enum and vise versa)
```
public enum CookieTypes
{
	ZaansHuisje = 0,
	Deugnietje,
	Biscuit,
}

public static int32 Main(void)
{
	int32 a = (int32)CookieTypes.ZaansHuisje;
	float32 b = (float32)CookieTypes.Deugnietje;
	CookieTypes c = (CookieTypes)a;
	CookieTypes d = (CookieTypes)b;

	return 0;
}
```

Converting to lower precision types decreases the value's precision

Example
```
public static int32 Main(void)
{
	float64 a = 1.0;
	float64 b = 2.0;
	float32 c = (float32)a + (float32)b;

	return 0;
}
```

Implicit conversion is not allowed

Bad (implicit conversion)
```
public static int32 Main(void)
{
	int32 a = 1.0;
	float32 b = 2.0;
	float64 c = a + b;

	return 0;
}
```