# Node-Express-JS-Notebook
Notes for Node js and Express js

## Key concepts
* __dirname: gives us the path of our directory
* __filename: gives us the path of our file
* require(): function for importing
* Working with modules
  
## Exporting items using module.exports

For single item exposts:

```javascript
const sayHi = (name) => {console.log(`Heyy there ${name}`)}
module.exports = sayHi;
```
For multiple item exports (one way):

```javascript
const PI = 3.14
const USER = "Bushra"

module.exports = { PI, USER}
```

