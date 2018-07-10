### Types
**Value types** | **C# type**
--------------- | ------------
```bit```		| ```bool```
```enum```		| ```enum```
```float32```	| ```float```
```float64```	| ```double```
```float128```	| ```decimal```
```int8```		| ```sbyte```
```int16```		| ```short```
```int32```		| ```int```
```int64```		| ```long```

** Reference types** | **Function**
-------------------- | ------------
```class```			 | custom data type
'''function'''		 | function pointer
```void```			 | no type

#### Notes
- ```bit```			The bit is only 1 bit in size, and can only be 1 or 0
- ```float(x)```	The float(x) is a floating point value, and it's size is x bytes
- ```int(x)```		The int(x) can only be a decimal number, and it's size is x bytes

- value types cannot be ```null```
- ```float(x)``` types can be casted to a different ```float(x)``` type at the loss of precision
- ```int(x)``` types can be casted to a different ```int(x)``` type at loss of precision
- only ```int(x)``` types can be ```unsigned```
- ```void``` functions do not have to return a valu