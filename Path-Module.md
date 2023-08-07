### path Module

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
