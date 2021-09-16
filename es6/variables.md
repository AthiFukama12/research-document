# Variables
Variable is the name of the storage location. There are two types of variables: local variable and global variable.

## var
The var keyword is used to define global variables:
* In var, you can redeclare the variable (you may change the variable later).
* You can access var globally.(we do not use this variable at Pragma).
* Variables with var can be reassigned and redeclared.
  * **Example 1**

```javascript
  //Declaring variable greet.
  var greet = "hey";
  //Redeclaring the variable. 
  var greet = "Hello"; 
  
  console.log(greet)
```
### The difference between local and global variables.
* **Local variables** - A local variable is only visible inside the block or body of the function.
  * **Example 2** 
```javascript
  function colour(){
  //Local variable.    
  var colourname = "Orange";
    console.log(colourname);
  }
  //Calling the function.
  colour();
```
  
* **Global variables.** - A global variable has a global scope which means that it is defined or accessible anywhere in the code.
  * **Example 3**
  
```javascript
  //Global variable.
  var horsename = "Blonde";
  /**
  * This function console log
  * @param {string} 
  */
  function colour(){
   console.log(horsename);
  }
  //Calling the function.
  colour();
```

## const
The const keyword is used to define constant variables:
* Variables with const cannot be reassigned and redeclared.
* Variables with const consist of block scope.
* Although const does not allow you to redeclare or reassign the variable, you can change the elements of const array.
  * **Example 4**
  
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
* Let also allows you to change the variable at a later stage.
  * **Example 5** 
  
```javascript
  //Declaring and assigning num1.
  let num1= 4;    
  
  //Assigning variable num1 (this means that the variable num1 will now change to 3).
  num1 = 3;    
  
  console.log(num1);

```








