
## Null and Undefined

-   Used to express 'nothing' in JavaScript.
    
-   If we declare a variable, and don't set anything to it, then it has value `undefined`.
    
    ```javascript
      let dog;
      console.log(dog); // undefined
    
    ```
    
    When we try to access a variable that is created but not defined/set a value, we get `undefined`.
    
-   **null:** value of nothing
    
    ```javascript
      const somethingNull = null;
      // we have explicitly set the value to be nothing with null
    ```