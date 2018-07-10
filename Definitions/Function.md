### Function
`function<`_`return type`_`>(`_`parameters`_`)`
The ```function``` type is a function pointer
- _return type_ is the return type of the function pointer
- _parameters_ are the accepted parameters of the function pointer

Example
```
function<void>(int32, int32) Foo
```
The function pointer "Foo" returns nothing, and needs two int32 parameter

To call the function pointer, just call the function as you normally would
```
Foo(3, 6);
```

Only functions that are implemented, have the same return types and have the same parameters can be assigned to the function pointer

Good
```
void FooFunction(int32 a, int32 b) { }

function<void>(int32, int32) Foo = null;

Foo = FooFunction;
```

Bad (return type)
```
int32 FooFunction(int32 a, int32 b) { return 0 }

function<void>(int32, int32) Foo = null;

Foo = FooFunction;
```

Bad (not matching parameters)
```
void FooFunction(int32 a, float64 b) { }

function<void>(int32, int32) Foo = null;

Foo = FooFunction;
```

Bad (abstract modifier)
```
abstract void FooFunction(int32 a, int32 b);

function<void>(int32, int32) Foo = null;

Foo = FooFunction;
```