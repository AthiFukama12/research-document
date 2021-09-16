# Scope
* Scope means available. A variable defined inside a scope is accessible only within that scope,but inaccessible outside.
* In JavaScript, scopes are created by code blocks and functions.

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
  //Declaring and assigning variable employeeName.
  let employeeName = "Ace"; 
  employeeName = "Athi";
  //This function takes one parameter called value.
  function employee(value){
  //Displays value of function on the console.
    console.log( "Employee name: ", value); 
  }
  //Takes value of employeeName (outside function).
  employee(employeeName);                      
  console.log("Employee name", employeeName);   
```
   
### Block scope
* Declaring a variable inside and outside  the curly brackets.
* Variable  inside the curly brackets cannot be accessed outside the  block.
* Let and const are default of block scope(which means let and const contains block scope).
* This code below will execute the error message "num2 is not defined"(because the variable is inside the {}).
  * **Example 3**
  
```javascript

    if (num1 == 1) {
        let num2 = 2;
    }
    //Num1 is not defined.
    console.log(num1);
```
  
* This code below will execute 3 because variable num = 3 because 3 is declared outside curly brackets.
  * **Example 4** 

```javascript
    let num1 = 3
    
    if(num1 == 3) {
        let num1 = 1;
    }
    //Output of 3 is expected.
    console.log(num1);   
```
 
