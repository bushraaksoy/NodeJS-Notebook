# Node-Express-JS-Notebook
Notes for Node js and Express js

## Key concepts
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

## path Module

```js
const path = require('path')
console.log(path.resolve(path))
```
this returns an absolute path of the paths specified

```js
const joinedPath = path.join(file1, file2, file3)
console.log(joinedPath)
```
returns a file path that has joined the the three files.
