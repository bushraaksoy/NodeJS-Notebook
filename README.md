# Node-Express-JS-Notebook
My notebook for learning nodejs and Expressjs

## Some facts
* __dirname: gives us the path of our directory
* __filename: gives us the path of our file
* require(): function for importing
* Working with modules
  
## Exporting items using module.exports

For single item exposts:

```js
const sayHi = (name) => {console.log(`Heyy there ${name}`)}
module.exports = sayHi;
```
For multiple item exports (one way):

```js
const PI = 3.14
const USER = "Bushra"

module.exports = { PI, USER}
```
