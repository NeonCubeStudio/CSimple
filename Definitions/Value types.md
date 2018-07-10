### Types
**Value types** | **C# type**
--------------- | ------------
```bit```		| ```bool```
```int8```		| ```sbyte```
```int16```		| ```short```
```int32```		| ```int```
```int64```		| ```long```
```float32```	| ```float```
```float64```	| ```double```
```float128```	| ```decimal```
```enum```		| ```enum```

#### Notes
- ```bit```			The bit is only 1 bit, and can only be 1 or 0
- ```int(x)```		The int(x) can only be a decimal number, and it's size is x bytes
- ```float(x)```	The float(x) is a floating point value, and it's size is x bytes

- value types cannot be ```null````
- only ```int(x)``` types can be ```unsigned```
- ```int(x)``` types can be casted to a different ```int(x)``` type at loss of precision
- ```float(x)``` types can be casted to a different ```float(x)``` type at the loss of precision