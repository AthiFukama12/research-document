# Variables
variable is the name of the storage location.


## var
The var keyword is used to define global variables:
* In var you can redeclare the variable (you may change the variable later)
* You can access var globally.(we do not use this variable at Pragma).
* Variables with var can be reassigned and redeclared.


Sample code of var.
* Example 1
    ```javascript
       var greet = "hey ";   //Declaring variable greet
       var greet = "Hello "; //Redeclaring the variable 
    
       console.log(greet)
    ```

## const
The const keyword is used define constant variables:

* variables with const cannot be reassigned and redeclare.
* Variables with const consist of block scope.
* Although const does not allow you to redeclare or reassign the variable, you can change the elements of const array.

Sample code of const
* Example 1
   ```javascript
      // Create an Array:
      const cars = ["Saab", "Volvo", "BMW"];
    
      // Change an element:
      cars[0] = "Toyota"; 
      console.log(cars);
    
   ```
## let
The let keyword is used define let variables:
* variables with let cannot be redeclared .
* let variables must be declared before the block code or use.
* let consist of block scope.
* let allows you to change the variable at a later stage.

Sample code of let
* Example 1 
  ```javascript
     let number = 4;    //Declaring and assigning x
     {
       number = 3;     //Assigning variable x(this means that the variable x will now change to 3)
     }
     console.log(number);
  ```







