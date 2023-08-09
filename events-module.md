# events Module
```js
const EventEmmiter = require('events')

const customEmmiter = new EventEmmiter()

customEmmiter.on('response', () => {
  console.log('data recieved')
})

customEmmiter.emit('response')
```

we can also use this event module instead of createServer

```js
const server = http.createServer()
server.on('request', (req, res) => {
  res.end('welccome') // and so on
})
