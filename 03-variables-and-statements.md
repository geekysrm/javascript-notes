## Variables and statements

Semicolons used to end a statement. You can choose to not write them _(because there is ASI: Automatic Semicolon Insertion in Javascript)_.

### Declaring a variable:

`var first = 'Soumya';`

`let first = 'Soumya';`

`const first = 'Soumya';`

(here value is 'Soumya')

-   `let` and `const` were introduced in ES6 (newer).
    
-   `var` and `let` can be updated but not `const`.
    
    ```javascript
      var x = 'hey';
      y = 'hi';
      
      let cool = true;
      cool = false;
      
      const age = 10;
      age = 11; // wrong: throws error
    
    ```
    
-   In **strict mode**, we have to define a variable first before assigning a value to it.
    
    ```javascript
      dog = 'snickers'; // bad coding, don't do this
      console.log(dog); // snickers (no error) 
      
      'use strict';
      dog = 'snickers'; // error: dog is not defined
    
    ```
    
-   If we write `var dog;` dog is _undefined._
    
-   **Scoping:**
    
    -   **var** : _function scoped_ (only available inside parent functions)
        
    -   **let** and **const** : _block scoped_ (available inside a block denoted by _{ }_ )
        
-   **Opinion (what to use):** Use `const` by default; if the value of the variable needs to change then use `let`. Almost never use `var`.
    
-   **Variable naming conventions:**
    
    -   Should not start with capital unless they are a _class_.
    -   Must start with **a-z** or **_** or **$**.
    -   If a variable is multi-word, you can use:
        -   _Camel-case:_ `let iLovePizza = true;`
        -   _Upper Camel case (in case of classes):_ `ILovePizza`
        -   _Snake case: `let i_love_pizza=true;`_