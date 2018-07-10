### Types
**Value types** | **C# type**
--------------- | ------------
```bool```		| ```bool```
```enum```		| ```enum```
```float32```	| ```float```
```float64```	| ```double```
```int8```		| ```sbyte```
```int16```		| ```short```
```int32```		| ```int```
```int64```		| ```long```

**Reference types** | **C# type**
-------------------- | ------------
```class```			 | ```class```
```function```		 | ```action```
```void```			 | ```void```

#### Description
- ```bool```		The ```bool``` is only 1 byte in size, and can only be 0 or 1
- ```enum```		The enum contains named constants, and each named constant is the same size as int64
- ```float(x)```	The ```float(x)``` is a floating point value, and it's size is x bits
- ```int(x)```		The ```int(x)``` can only be a decimal number, and it's size is x bits
- ```function```	The ```function``` type is a function pointer

#### Notes
- value types cannot be ```null```
- ```float(x)``` types can be casted to a different ```float(x)``` type at the loss of precision
- ```int(x)``` types can be casted to a different ```int(x)``` type at loss of precision
- only ```int(x)``` types can be ```unsigned```
- ```enum``` values are immutable
- ```enum``` and ```function``` types cannot be a pointer (i.e. function<void>(void)*, enum*)
- ```void``` is not a valid type for variables
- ```void``` functions do not have to use to use the ```return``` keyword to denote the end of a function