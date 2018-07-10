### Function pointer
Application.csimple
```
include System;		/* print function */

public class Test
{
	public int32 Combine(int32 a, int32 b)
	{
		return a + b;
	}
}

public static int32 Main(void)
{
	function<int32>(int32, int32) FunctionPointer = null;
	int32 a = 0;
	int32 b = 0;
	int32 result = 0;

	FunctionPointer = Test.Combine;

	if (FunctionPointer)
	{
		result = FunctionPointer(a, b);
		
		Print({0}, result);
	}

	return 0;
}
```