### String

-   used for holding text
    
-   3 ways to create strings:
    
    1.  using single quotes:
        
        `const first = 'Soumya';`
        
    2.  using double quotes:
        
        `const middle = "Ranjan";`
        
    3.  using backticks:
        
        ```javascript
         	const last = `Mohanty`;
        
        ```
        
-   single quotes and double quotes are the same thing.
    
    used for: `"she's cool"`
    
    or escaping: `'she\\'s cool'`
    
-   backticks:
    
    ```javascript
      const sentence = `she's so "cool"`;
      console.log(sentence); // she's so "cool"
    
    ```
    
-   Multi-line string:
    
    ```javascript
      const song = 'Oh \\
      I like \\
      pizza';
      
      console.log(song); // Oh I like pizza
    
    ```
    
    ```javascript
      const song = `Oh
      I like
      pizza`;
      
      console.log(song); 
      /*
      Oh
      I like
      pizza
      */
    
    ```
    
    2nd one using backticks is mostly used.
    
-   **String concatenation and interpolation**
    
    -   '+' is used for **concatenation**. It is also used for adding 2 nos.
    -   **Concatenation**: when 2 or more strings combined to one
    -   **Interpolation**: when you put a variable inside a string
    -   Example 1:
    
    `const name = 'Soumya';`
    
    `const hello = 'Hello my name is ' + name + '. Nice to meet you.'`
    
    _(can use double or single quotes)_
    
    -   Example 2:
        
       ` 1+1 // 2`

	 `'1'+'1' // 11 `

	`1 + '1' // 11`
        
    -   Example 3:
        
        const name = 'Soumya'; const hello = `Hello my name is ${name}. Nice to meet you. I am ${100+1} years old.`; console.log(hello); // Hello my name is Soumya. Nice to meet you. I am 101 years old.
        
    -   Backticks also used for _tagged template literals_.
        
    -   Backticks are helpful for creating HTML:
        
        ```javascript
          const html = `
          	<div>
          		<h2>Hey everyone! I am ${name}.</h2>
          	</div>
          `;
        ```