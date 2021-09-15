# Arrow Functions

* Arrow functions allow us to write shorter function syntax.
* You cannot use arrow function in a constructor
* They cannot be called with the new keyword. Doing that throws an error indicating that the function is not a constructor.


```javascript
    //Declaring variable
    var hello;             
    
    //Remove the word "function" and place arrow between the argument and opening body bracket.
    hello = () =>{
        console.log('Hello');
    }
    hello();
```
```javascript

    let firstname;
    let  lastname;
    
    //Takes two String parameters.
    function person(firstname,lastname){
        //Prints the values on the console.
        console.log(firstname + lastname)  
    
    }
    //Passes two parameters to the person() function.
    person('Athi ', 'Fukama');             
```

```javascript
    //Remove the word "function" and place arrow between the argument and opening body bracket
    const speak = () =>{
    console.log("good day");
    };
    //Calling the function
    speak();                   
```

## Normal function
### Here I was curious, because I wanted to see the difference between arrow and normal function
```javascript
    //Declaring the function
    function greet(){
        console.log("hello world");
    }
    //Calling the function
    greet();                          

```

```javascript
    //Function expression
    const speak = function(){
    console.log("good day");
    };
    //Calling the function
    speak();                   
```