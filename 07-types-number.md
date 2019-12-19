
## Number

Only **one** type of number in JavaScript whether it has decimal point or not.

```javascript
const age = 100;
const money = 1000.50
console.log(typeof age); // number
console.log(typeof money); // number

```

-   `typeof` is used to find out the 'type' of a variable.
    
-   Various operations: addition, subtraction, multiplication, division can be done with nos.
    
-   Example
    
    `"10" * "10" // 100 (number) - converts the strings to number`
    

The above works with _multiplication, division and subtraction and not addition,_ because the + sign is also used for concatenation.

-   **Math helper methods:**
    
    -   **Math.round, Math.floor, Math.ceil, Math.random** and many others
        
        ```javascript
          Math.round(2.5); // 3
          Math.floor(2.4); // 2
          Math.ceil(2.4); // 3
          Math.random(); // 0.565262543048269 - random no. between 0 and 1
        
        ```
        
-   **Modulo and Power operators:**
    
    ```javascript
      const smarties = 20;
      const kids = 3;
      const eachKidGets = Math.floor(smarties/kids); // 6
      const leftSmarties = smarties % kids; // 2 - modulo operation
      
      const x = 2 ** 3; // 8 - power operation using power operator (**)
      // or
      const x = Math.pow(2,3); // 8 - power operation using Math.pow
    
    ```
    
-   Example
    
    0.1 + 0.2 // 0.30000000000000004
    

Why? [Explanation](http://0.30000000000000004.com/)

So, when working with money, don't store them as dollars and cents. Store all of the money in cents as you won't have to deal with fractions only whole nos. When need to display to user, just convert them back.

-   **Infinity and Negative Infinity:**

`typeof Infinity; // number`

`typeof -Infinity; // number`

-   **Not a Number (NaN):**

`10 / 'dog' // NaN`

`typeof NaN // number`