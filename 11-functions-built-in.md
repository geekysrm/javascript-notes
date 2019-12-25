## Functions - Built in

-   Function allows us to _group together multiple statements,_ take in some values, perform some operations and return some value.
    
-   Functions take in data known as _arguments._
    
-   Function may or may not _return_ a value.
    
-   Example:
    
    ```javascript
      Math.max(10, 12); // 12
    
    ```
    
    The above line is a JavaScript statement.
    
    10 and 12 passed to the function are arguments, separated by comma.
    
    12 is _returned_ from the function.
    
-   There are many in-built JavaScript functions.
    
    e.g:
    
    -   `console.log('hey');` returns `undefined` , logs `hey`.
    -   `parseFloat('2.032565') // 2.032565` (converts string to number)
    -   `parseInt('2.032565') // 2` (converts string to number as integer)
    -   Many date functions are also present. e.g. `Date.now()` returns no. of milliseconds since January 1, 1970 00:00:00 UTC.
    -   DOM functions:
        -   Example:
            
            ```html
              <body>
              <p>Hey How ya doin?</p>
              	<script>
              		const para = document.querySelector('p'); // finds p tag in page
              		console.log(para); // <p>Hey How ya doin?</p>
              	</script>
              </body>
            
            ```
            
        -   Mobile only functions e.g. `navigator.vibrate()`
            
-   In case of doubts, always refer MDN Docs.
    
-   Other Examples:
    
    ```javascript
      scrollTo(0, 200); // scrolls to (x, y) position in page
      
      scrollTo({
      	top: 500,
      	left: 0,
      	behavior: 'smooth'
      }); // scrolls to position top: 500, left: 0 in a 'smooth' manner
    
    ```
    
    The `scrollTo` function returns `undefined`.