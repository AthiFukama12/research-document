# Scope
* Scope means available.A variable defined inside a scope is accessible only within that scope,but inaccessible outside.
* In JavaScript,scopes are created by code blocks and functions.

## Three different types of scope

### Global scope
* Variables that are declared outside the function have a global scope.
* Global variables can be assessed anywhere in javascript program.
  * **Example 1**
  
```javascript
  let carName = "Volvo";
  //Code here can use carName.
  myFunction();
  
  function myFunction() {
    console.log(carName);
  //Code here can also use carName.
  }
```

### Functional scope
 * Functional means a function is available.
 * Variables declared inside the function are not visible or accessed outside the function.
   * **Example 2**
  
```javascript
  //Declaring and assigning variable employeeName .
  let employeeName = "Ace"; 
  employeeName = "Athi";
  //This function takes one parameter called value.
  function Employee(value){
  //Displays value of function on the console.
    console.log( "Employee name: ", value); 
  }
  //Takes value of employeeName (outside function).
  Employee(employeeName);                      
  console.log("Employee name", employeeName);   
```
   
### Block scope
* Declaring a variable inside and outside  the curly brackets.
* Variable  inside the curly brackets cannot be accessed outside the  block.
* Let and const are default of block scope(which means let and const contains block scope).
* This code below will execute the error message "number is not defined"(because the variable is inside the {}).
  * **Example 3**
  
```javascript
  {
  let number = 2;
  }
  console.log(number);
  // number can NOT be used here()
```
  
* This code below will execute 3 because variable number = 3 is declared outside curly brackets.
  * **Example 4** 

```javascript
  let number = 3
  {
    let number = 1; 
  }
  console.log(number);
```
 
