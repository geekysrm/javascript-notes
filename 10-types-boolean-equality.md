## Booleans and Equality

-   A **boolean** variable can be either `true` or `false` .
    
-   Example:
    
    ```javascript
      const age = 18;
      const ofAge = age > 18;
      console.log(ofAge); // false
    
    ```
    
-   **Equal signs:**
    
    -   `=` sign: used for assignment/ updation of values
        
        ```javascript
          let name = 'Soumya';
          name = 'Raja';
        
        ```
        
    -   Out of `==` and `===`, you should **almost always** use `===`.
        
    -   `==` and `===` are used for equality comparison.
        
        ```javascript
          console.log(age === 18); // true
        
        ```
        
    -   `==` vs `===` :
        
        `===` checks both **type & value.**
        
        `==` only checks **value.**
        
        ```javascript
          10 === "10" // false as values are same but types are not
          10 == "10" // true as values are same
        
        ```
        