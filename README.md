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
```

### resolve()
```js
const absolutePath = path.resolve(path)
console.log(absolutePath)
```
this returns an absolute path of the paths specified

### join()
```js
const joinedPath = path.join(file1, file2, file3)
console.log(joinedPath)
```
returns a file path that has joined the the three files.

### basename()
```js
const fileName = path.basename(path)
console.log(fileName)
```
reurns the base name of the file path

### sep()
```js
console.log(path.sep)
```
returns the separator for the file paths

## fs Module

```js
const fs = require('fs')
```
### readFileSync()
```js
// standard encoding type is 'utf-8'
const file = fs.readFileSync(fileName, encodingType)
console.log(file)
```
this code will print out all the contents of the filename specified

### writeFileSync()
```js
fs.witeFileSync(filePath, content)
```

This will create a new file with the path specified and with the name specified at filePath, and add the content specified inside it.

```js
fs.writeFileSync(filePath, content, {flag: a}
```

