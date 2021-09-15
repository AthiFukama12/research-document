# Variables
Variable is the name of the storage location.

## var
The var keyword is used to define global variables:
* In var, you can redeclare the variable (you may change the variable later)
* You can access var globally.(we do not use this variable at Pragma).
* Variables with var can be reassigned and redeclared.
  * **Example 1**

```javascript
  var greet = "hey ";   //Declaring variable greet
  var greet = "Hello "; //Redeclaring the variable 
  
  console.log(greet)
```

## const
The const keyword is used to define constant variables:
* Variables with const cannot be reassigned and redeclared.
* Variables with const consist of block scope.
* Although const does not allow you to redeclare or reassign the variable, you can change the elements of const array.
  * **Example 2**
```javascript
  //Create an Array:
  const cars = ["Saab", "Volvo", "BMW"];
  
  //Change an element:
  cars[0] = "Toyota"; 
  console.log(cars);
```

## let
The let keyword is used to define let variables:
* Variables with let cannot be redeclared.
* Let variables must be declared before the block code or use.
* Let consist of block scope.
* Let allows you to change the variable at a later stage.

  * **Example 3** 
```javascript
  //Declaring and assigning number
  let number = 4;    
  {
    //Assigning variable number(this means that the variable number will now change to 3)
    number = 3;    
  }
  console.log(number);

```








