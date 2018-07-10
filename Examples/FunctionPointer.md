### Function pointer
Test.csimple
```
include System;		/* print function */

public class Test
{
	public void OutputText(void)
	{
		Print("Hello world!");
	}
}
```
Application.csimple
```
public static int32 Main(void)
{
	function<void>(void) FunctionPointer = Test.OutputText;

	if (FunctionPointer)
	{
		FunctionPointer();
	}

	return 0;
}
```