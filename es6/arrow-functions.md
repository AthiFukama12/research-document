# Arrow Functions

* Arrow functions allow us to write shorter function syntax.
* You cannot use arrow function in a constructor.
* They cannot be called with the new keyword. Doing that throws an error indicating that the function is not a constructor.
* There is no big difference between  arrow and normal function because they execute the same output.


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
    
    /**
     * This function console log
     * @param {string} firstname - the firstname of the person.
     * @param {string} lastname - the lastname of the person.
     */
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
