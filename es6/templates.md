# Template literals
* Template literals uses back-ticks (``) to define a string.
* **Example 1**

```javascript
  let text = `Hello world!`;
  console.log(text);
```

* Template literals are not supported by Internet Explorer.
* With template literals you can use both single and double quotes inside a string.
  * **Example 2**
  
```javascript
  let text = `Hello, My name is "Athi"`;
  console.log(text);
```

* Template literals allows multiline strings.
  * **Example 3**
  
```javascript
  let text = 
  `The quick
  brown fox
  jumps over 
  the lazy dog`
  console.log(text);
```

* Template literals provides an easy way to interpolate variables and expression into strings. The method is called string interpolation(${...}).
* Template literals allows variables in strings(variable substitutions).
  * **Example 4**
  
```javascript
  //Declaring  variables  
  let firstName = "John";
  let lastName = "Doe";
  
  let text = `Welcome ${firstName}, ${lastName}`
  console.log(text);
```
 
* Template literals also allows expressions in strings:
  * **Example 5**
  
```javascript
  //Declaring variables.
  let price = 20.00
  let tax = 0.25
  
  
  let total = `The total price is ${price *tax}`;
  console.log(total);
```
