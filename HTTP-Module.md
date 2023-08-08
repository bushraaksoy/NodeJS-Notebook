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
```js
 const server = http.createServer((request, response) => {
    if(request.url === '/'){
      response.end("Hello and welcome to our home page")
    }
    if(request.url == '/about/'){
      response.end('Hello this is our about page')
    }
    response.end(
    `
      <h1>Opps there was an error!</h1>
      <a href="/">home page</a>
    `
    )
  })
```
This outputs the given messages to the screen depending on the path specified, and if someone navigates to a non existing page, it outputs the default html page.
