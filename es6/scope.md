# Scope
* Scope means available

## Three different types of scope

### Global scope
* Variable that are declared outside the function have a global scope.
  * Global variables can be assessed anywhere in javascript program.
    * Example 1
      ```javascript
         let carName = "Volvo";
         // code here can use carName
         myFunction();
  
         function myFunction() {
         console.log(carName);
         // code here can also use carName
         }
     ```
  
### Functional scope
 * functional means a  function is available
 * Variables declared inside the function are not visible or accessed outside the function.
   * Example 1
      ```javascript
         let employeeName = "Ace"; //Declaring and assigning variable employeeName 
         employeeName = "Athi";    //Assigning employeeName(the previous value which is Ace will be replaced with Athi)
    
         function Employee(value){                      //This function takes one parameter called value
           console.log( "Employee name: ", value);    //Displays value of function on the console
         }
    
         Employee(employeeName);                       //Takes value of employeeName (outside function).
         console.log("Employee name", employeeName);   //Displays employeeName on console
      ```
   
### Block scope
Declaring a variable inside and outside  the curly brackets.
* Variable  inside the curly brackets cannot be accessed outside the  block.
* let and const are default of block scope(which means let and const contains block scope).
  * Example 1
    * This code below will execute the error message "number is not defined"(because the variable is inside the {}).
    ```javascript
       {
         let number = 2;
       }
       console.log(number);
       // number can NOT be used here()
    
    ```
  
* This code below will execute 3 because variable number = 3 is declared outside curly brackets.
  * Example 2 
    ```javascript  
       let number = 3
       {
         let number = 1; 
       }
       console.log(number);
    ```
