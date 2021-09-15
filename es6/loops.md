# Loops
* Looping in programming  languages is a feature which facilitates the execution of a set of instructions/functions repeatedly while some condition evaluates to true. 
## The For Of Loop
* The JavaScript for of statement loops through the value of an iterable object.
* It let you loop over iterable data structures such as arrays,strings,set, map and more:
### Syntax

```html
for (variable of iterable) {
    // code block to be executed
 }
```
* **Variable** - For every iteration the value of the next property is assigned to the variable.Variable can be declared with const, let or var.
* **Iterable** - An object that has iterable properties.The iterable protocol allows JavaScript objects to define or customize their iteration behavior, such as what values are looped over in a for... of construct.
### Examples
* Iterating over an Array.
```javascript
    const array = [10,30,60];
    
    for (const value of array){
        console.log(value);
    }
```
* Iterating over a String

```javascript
    const iterable = "Athi"
    
    for (const value of iterable) {
      console.log(value);
      
    }
```
* Iterating over a Set

```javascript
    const iterable = new Set([1, 1, 2, 2, 3, 3, 4, 4]);
    
    for (const value of iterable) {
      console.log(value);
      
    }
```
* Iterating over a map
```javascript
    const iterable = new Map([['a', 1], ['b', 2], ['c', 3]]);
    
    for (const value of iterable) {
      console.log(value);
      
    }
    for (const [key, value] of iterable) {
        console.log(value);
    }
```