# HTTP Module

```js
const http = require('http');
```

* createServer() Creating a server
  ```js
  const server = http.createServer((request, response) => {
    if(request.url === '/'){
      response.end("Hello and welcome to our home page")
    }
  })
  ```
* server.listen
```js
server.listen(port);
```
this one runs the server on the specified port for eg server.listen(5000)
```
