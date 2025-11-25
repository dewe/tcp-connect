# tcp-connect

Check if a TCP port is reachable. Returns connection time in milliseconds.

## Usage

```javascript
var tcp = require('tcp-connect');

tcp(google.com, 80, 1000)
  .then(() => console.log('google.com is available'))
  .catch(() => console.log('no luck this time'));
```

## Development

Tests are best run in docker:

```shell
docker-compose run tcp-connect npm test
```
