# fs Module

```js
const fs = require('fs')
```

## Syncronous functions

* readFileSync()
```js
// standard encoding type is 'utf-8'
const file = fs.readFileSync(fileName, encodingType)
console.log(file)
```
this code will print out all the contents of the filename specified

* writeFileSync()
```js
fs.witeFileSync(filePath, content)
```

This will create a new file with the path specified and with the name specified at filePath, and add the content specified inside it.

```js
fs.writeFileSync(filePath, content, {flag: a}
```
__ readFIleSync and writeFileSync are both <b>syncronous</b> and next is readFile and writeFile which are <b>asyncronous</b> __

## Asyncronous Functions

*readFile()
```js
fs.readFile(filePath, encoding, callback(err, result))
```
here this in an asyncronous function which returns either an error or the data in the file

*writeFile()
```js
fs.writeFile(filePath, content, callback(err, result))
```

__ these two functions are asynchronous __
