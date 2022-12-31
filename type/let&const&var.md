# let

1. Variables defined with let cannot be Redeclared.

``` 
let x = "John Doe";

let x = 0;

// SyntaxError: 'x' has already been declared
```
with var we can:
``` 
var x = "John Doe";

var x = 0;
```
2. Variables defined with let must be Declared before use.

3. Variables defined with let have Block Scope.

-----------------------------------------------------------------
# const
1. Variables defined with const cannot be Redeclared.

2. Variables defined with const cannot be Reassigned.

3. Variables defined with const have Block Scope.<br>
<br>
<br>
<br>
<br>
<br>
   Use const when you declare:

- A new Array
- A new Object
- A new Function
- A new RegExp

It does not define a constant value. It defines a constant reference to a value.

Because of this you can NOT:

- Reassign a constant value
- Reassign a constant object
- Reassign a constant array
But you CAN:

- Change the elements of constant array
- Change the properties of constant object


``` 
var x = 2;     // Allowed
const x = 2;   // Not allowed

{
let x = 2;     // Allowed
const x = 2;   // Not allowed
}

{
const x = 2;   // Allowed
const x = 2;   // Not allowed
}
```

``` 
const x = 2;     // Allowed
x = 2;           // Not allowed
var x = 2;       // Not allowed
let x = 2;       // Not allowed
const x = 2;     // Not allowed

{
  const x = 2;   // Allowed
  x = 2;         // Not allowed
  var x = 2;     // Not allowed
  let x = 2;     // Not allowed
  const x = 2;   // Not allowed
}
```