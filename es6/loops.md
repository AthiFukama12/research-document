# Loops
* Looping in programming languages is a feature which facilitates the execution of a set of instructions/functions repeatedly while some condition evaluates to true. 
## The For Of Loop
* The JavaScript for of statement loops through the value of an iterable object.
* It let you loop over iterable data structures such as arrays, strings, set, map and more:
### Syntax
 
```html
    for (variable of object) {
        // code block to be executed
    }
```
* **Variable** - For every iteration the value of the next property is assigned to the variable. Variable can be declared with const, let or var.
* **Iterable** - An object that has iterable properties. The iterable protocol allows JavaScript objects to define or customize their iteration behavior, such as what values are looped over in a for... of construct.
### Examples

* Iterating over an Array.
```javascript
    //Declaring an array.
    const array = [10,30,60];
    
    /**
    * This function console log.
    * @param {number} - value of the array.
    */
    for (const value of array){   
     console.log(value);
    }
```

* Iterating over a String.
```javascript
    //Declaring variable name.
    const name = "Athi"

    //Looping through the values of name.
    for (const value of name) {  
      console.log(value);
    }
```

* Iterating over a Set.
```javascript
    //Declaring a set of numbers.
    const numbers = new Set([1, 1, 2, 2, 3, 3, 4, 4]);

    //Looping through the values of numbers.
    for (const value of numbers) {                      
      console.log(value);
    }
```

* Iterating over a Map.
```javascript
    //Declaring  alphabets with values.
    const alphabetMap = new Map([['a', 1], ['b', 2], ['c', 3]]);   

    //Looping through the values of alphabetMap.
    for (const value of alphabetMap) {                            
      console.log(value);
    }
    
```