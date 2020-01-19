## Different ways of declaring functions

- Functions are **First class citizens:**

  - It means JavaScript functions are values in themselves. They can be stored in variables and passed into other functions, just like any other piece of data in JavaScript. (see 3rd example below)

- **With function keyword**

  _Important:_ These are **hoisted**, meaning JavaScript 'hoists' or puts them at the top of the file. So if we try to run a function defined with function keyword before it is defined/ above its definition, there's no error and the function is executed successfully.

  ```javascript
  function doctorize(firstName) {
    return `Dr. ${firstName}`;
  }
  ```

- **Anonymous function - function with no name**

  These are used in _callbacks_ and _IIFE: immediately invoked function expressions_.

  ```javascript
    function (firstName) {
     return `Dr. ${firstName}`;
    }

  ```

- **Function Expression**

  _Important:_ These are **not hoisted**, meaning JavaScript doesn't put them at the top of the file. So if we try to run a function not defined with function keyword before it is defined/ above its definition, there's an error and the function fails to execute.

  ```javascript
  const doctorize = function(firstName) {
    return `Dr. ${firstName}`;
  };
  ```

- **Arrow Functions**

  - Concise, shorter syntax

  - Don't have own scope in refer to 'this' keyword

  - Are anonymous functions

    ```javascript
    const inchToCM = inches => {
      return inches * 2.54;
    };

    // Implicit return: const add = (a, b = 3) => a + b; const inchToCM = (inches) => inches * 2.54;

    // In case of only 1 parameter, we can omit the () around it const inchToCM = inches => inches * 2.54;
    ```

  - Implicitly returning an object:

    ```javascript
    const makeABaby = (first, last) => ({ name: `${first} ${last}`, age: 0 });
    ```

- **IIFE: Immediately Invoked Function Expression**

  ```javascript
  (function(age) {
    return `You are cool and age ${age}`;
  })(10);

  // Parantheses run first in JavaScript, so we have wrapped the function in ().
  // The function immediately runs.
  // The argument passed here is 10 for parameter age.
  ```

- **Methods:**

  - A function which lives inside an object.

  - For e.g `console.log('hey')` : here `log` is the function and `console` is the object.

  - **2 Ways to define methods:**

    ```javascript
    const wes = {
      name: "Westopher Bos",
      // Method!
      sayHi: function() {
        console.log(`Hey ${this.name}`);
        return "Hey Wes";
      },
      // Arrow function
      wisperHi: () => {
        console.log("hii wesss im a mouse");
      },
      // Short hand Method
      yellHi() {
        console.log("HEY WESSSSS");
      }
    };
    ```

- **Callback functions:**

  - Function that is passed to another function used for something that will happen when something is done.

```
HTML:
	<body>
        <button class="clickMe">
	        Click Me!
        </button>
   </body>





     Javascript:
        // Click Callback const button = document.querySelector('.clickMe');

        function handleClick() { console.log('Great Clicking!!'); }

        button.addEventListener('click', handleClick); // everytime we click the button, the handleClick function is run.

        button.addEventListener('click', function() { console.log('Nice Job!!!'); }); // everytime we click the button, the function inside is run.

        // Timer Callback setTimeout(() => { console.log('DONE! Time to eat!'); }, 1000); // it runs the console.log after each 1 sec or 1000 milliseconds
```
