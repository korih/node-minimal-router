# node-router

This is a minimal node router with no external dependencies. It is useful for small projects where you want to setup a server with some endpoints but don't want to use express. 


There is only two functions in this class, one for creating a path and one for handling requests.

To have the router handle requests you simply attach it to the node server.

```javascript
const server = http.createServer((req, res) => {
  router.handleRequest(req, res);
});
```

and then you can define a path for the router like so.

```javascript
const router = require('node-minimal-router')
router.createPath('/', (req, res) => {
  ...
  }
);
```
