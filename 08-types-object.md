
## Object

-   Everything in JavaScript is an Object.
    
-   Objects are used for collection of data, collection of functionality.
    
-   Example:
    
    ```javascript
      const person = {
      	name: 'Soumya', // property: value
      	age: 100
      };
      
      typeof person // object
      
      person.age = 101;
      console.log(person.age); // 101
    
    ```
    

.

-   Order of properties doesn't matter in an object.
-   **Accessing properties:**
    -   `person.name // Soumya` (dot notation)