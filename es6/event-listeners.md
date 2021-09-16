# Event listeners

## What is an event?
* Javascript's interaction with HTML is handled through events that occur when the user or the browser manipulates the page.
* When the page loads, it is called an event.When the user clicks a button,that click too is an event.

## Add event listener() method
* The addEventListener() method attaches an event handler to the specified element.
* The addEventListener() method attaches an event handler to an element without overwriting existing event handlers.
* You can add many event handlers to one element.
* You can add event handlers of the same type to one element.
* You can add event listeners to any DOM (Document Object Model),not only HTML elements.
* The addEventListener() makes it easier to control how the events reacts on bubbling.
* When using addEventListener() method,the JavaScript is separated from the HTML markup, for better readability and allows you to add even listeners even when you do not control the HTML markup.
* You can easily remove the event listener by using removeEventListener() method.
* Add an event listener that fires when the user clicks on a button.

### Examples
* **Example 1**
  * This example uses the addEventListener() method to attach a click event to a button.
  
```html
    <button id = "btn"> Try me</button>
```

```javascript
    const btn = document.querySelector("#btn")
    
    function display(){
    alert("Hello World!");
    }
    btn.addEventListener("click", display);
```
     
* **Example 2**
  * The addEventListener() method allows you to add many events to the same element, without overwriting existing events.
    
```html
    <button id = "btn"> Try me</button>
```

```javascript
  const myBtn = document.querySelector("#btn");
  myBtn.addEventListener("click", myFunction);
  myBtn.addEventListener("click", someOtherFunction);
  
  function myFunction() {
  alert ("Hello World!");
  }
  
  function someOtherFunction() {
  alert ("This function was also executed!");
  }
```

* **Example 3**
  * This example uses the addEventListener() method to add many events on the same button. 
```html
  <button id="btn">Try it</button>
  <p id="demo"></p>
```

```javascript
  const myBtn = document.getElementById("btn");
  myBtn.addEventListener("mouseover", myFunction);
  myBtn.addEventListener("click", mySecondFunction);
  myBtn.addEventListener("mouseout", myThirdFunction);
  
  function myFunction() {
  document.getElementById("demo").innerHTML += "Moused over!<br>";
  }
  
  function mySecondFunction() {
  document.getElementById("demo").innerHTML += "Clicked!<br>";
  }
  
  function myThirdFunction() {
  document.getElementById("demo").innerHTML += "Moused out!<br>";
  }
```

* **Example 4**
  * This example demonstrates how to pass parameter values when using the addEventListener() method.
  
```html
  <button id="btn">Try it</button>
 
```

```javascript
  let num1 = 5;
  let num2 = 7;
  
  const btn = document.querySelector("#btn")
  myFunction(num1, num2);
  
  function myFunction(a, b) {
  console.log(a*b);
  }
  btn.addEventListener("click", myFunction);
```
 