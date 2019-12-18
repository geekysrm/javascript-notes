## Running JavaScript:

- We can run JS on the browser's console by which we will have access to the page we are on.

- Also we can run it in a `script` tag:

```javascript
<script>console.log('Heyyy');</script>
```

Always try to have your `script` tag before the closing `body` tag, because we can access the HTML elements written above the `script` tag as they are above the JS.

- Also, we can run JS in another file using `script` tag with `src` attribute:

```javascript
<script src="relative path to js file"></script>
```

- Also we can run it via Node.js - instead of running in the context of a website we run it in an actual machine. In console, run: `node file.js`
