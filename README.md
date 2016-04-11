# tcp-connect
Check once for TCP connection.

# Install

```
npm install tcp-connect
```

# Usage

```javascript
var tcp = require('tcp-connect');

tcp(google.com, 80, 1000)
  .then(() => console.log('google.com is available'))
  .catch(() => console.log('no luck this time'));
```

# Development

Tests are best run in docker:

```
docker-compose build
docker-compose run tcp-connect npm test
```
