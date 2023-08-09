# Streams

```js
const { createReadStream } = require('fs')

const stream = createReadStream(filepath)
stream.on('data', (result) => {
  console.log(result)
})
// ... incomplete
```
