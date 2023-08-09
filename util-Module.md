# util Module

Makes asyncronous functions like readFile and writeFile return promise, and only when they are resolved.

```js
const util = require('util')
```

istead of creating a function and manualy returning a new promise, we apply this.
now we can use the util.promisify()
```js
const readFilePromise = util.promisify(readFile)

try{
  const fileContent = await readFilePromise(filepath, encoding)
  console.log(fileContent)
}
catch (err){
  console.log(err)
}
```

we can do the same thing with writefile

## An easier way to do this is by adding .promises in the end while we import the fs module.

```js
const fs = require('fs').promises
```
now they return the same thing but its more simple and we can just directly use the readFile and writeFile.
