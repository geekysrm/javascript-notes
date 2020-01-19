## Functions - arguments and parameters

- Parameters are like _placeholders_ for data that will be passed to a function.

- Arguments are the actual values passed to a function while calling it

  ```javascript
  function calculateBill(billAmount, taxRate) { // here billAmount, taxRate are parameters const total = billAmount + billAmount * taxRate return total; }

  calculateBill(100, 0.13); // here 100, 0.13 are arguments
  ```

![https://res.cloudinary.com/geekysrm/image/upload/v1576699296/parameters-arguments.jpg](https://res.cloudinary.com/geekysrm/image/upload/v1576699296/parameters-arguments.jpg)

- Parameters are variables local to the function; available only inside the function.

- You can also pass variables as arguments during a function call.

- We can also pass _expressions_ as arguments to a function.

  ```
    myTotal3 = calculateBill(20+20+30, 0.3);

  ```

- So, we can either pass direct value or variables holding value or expressions resulting in a value to a function as arguments.

- **Passing functions as arguments:**

  ```javascript
  function doctorize(name) {
    return `Dr. ${name}`;
  }

  function yell(name) {
    return `HEY ${name.toUpperCase()}`;
  }

  // We can pass a function inside another
  yell(doctorize("Soumya")); // HEY DR. SOUMYA
  // Above, returned value of doctorize function is passed to yell function
  ```

  - Default values:

    ```javascript
    function yell(name = "Silly Goose") {
      return `HEY ${name.toUpperCase()}`;
    }

    yell("Soumya"); // HEY SOUMYA
    yell(); // HEY SILLY GOOSE

    // Above, if we don't pass any argument to yell function, then it takes the default value in function definition,
    // here Silly Goose, else it takes whatever we pass as argument.
    ```

  - **Important gotcha:**

    ```javascript
    function calculateBill(billAmount, taxRate = 0.13, tipRate = 0.15) {
      console.log("Running Calculate Bill!!");
      const total = billAmount + billAmount * taxRate + billAmount * tipRate;
      return total;
    }

    // Suppose above, we want to pass the tipRate but not the taxRate and want taxRate to be default,
    // then the only thing we can do is:

    calculateBill(100, undefined, 0.66); // here the taxRate will default to 0.13 as
    // we have passed undefined to it and the tipRate will be 0.66 as passed
    ```
