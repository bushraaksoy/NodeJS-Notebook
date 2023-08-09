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
