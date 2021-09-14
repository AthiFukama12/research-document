# Template literals
* Template literals uses back-ticks (``) to define a string.
  * Example
    ```javascript
       let text = `Hello world!`;
       console.log(text);
    ```
* Template literals are not supported by Internet Explorer.
  * With template literals you can use both single and double quotes inside a string.
    * Example
    ```javascript
      let text = `Hello, My name is "Athi"`;
      console.log(text);
    ```
  * Template literals allows multiline strings.
    * Example
    ```javascript
       let text = 
       `The quick
       brown fox
       jumps over 
       the lazy dog`
       console.log(text);
    ```
* Template literals provide and easy way to interpolate variables and expression into strings. The method is called string interpolation(${...}).
  * Template literals allows variables in strings(variable substitutions)
    * Example
    ```javascript
       let firstName = "John";
       let lastName = "Doe";
  
       let text = `Welcome ${firstName}, ${lastName}`
       console.log(text);
    ```
* Template literals also allows expressions in strings:
  * Example
    ```javascript
       let price = 20.00
       let tax = 0.25
  
       let total = `The total price is ${price *tax}`;
       console.log(total);

    ```