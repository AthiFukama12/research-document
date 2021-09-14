# Arrow Functions
## Arrow function
* Arrow functions allow us to write shorter function syntax.
* You can not use arrow function in a constructor
* They cannot be called with the new keyword. Doing that throws an error indicating that the function is not a constructor.


```javascript
    var hello;             //Declaring variable
    
    //Remove the word "function" and place arrow between the argument and opening body bracket
    hello = () =>{
      console.log('Hello');
    }
    hello();
```
```javascript

    let firstname;
    let  lastname;
    function person(firstname,lastname){    //Takes two String parameters.
    
        console.log(firstname + lastname)  //prints the values on the console.
    
    }
    person('Athi ', 'Fukama');             //passes two parameters to the person() function.
```

```javascript
    //Remove the word "function" and place arrow between the argument and opening body bracket
    const speak = () =>{
    console.log("good day");
    };                         //when we use function expression,you put semicolon at the end of the function
    speak();                   //Calling the function
```

## Normal function
### Here I was curious, because I wanted to see the difference between arrow and normal function
```javascript
    //Declaring the function
    function greet(){
        console.log("hello world");
    }
    greet();                          //Calling the function

```

```javascript
    //function expression
    const speak = function(){
    console.log("good day");
    };                         //when we use function expression,you put semicolon at the end of the function
    speak();                   //Calling the function
```