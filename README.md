# express-json-status-codes

Extend the Express response object to set the status code and return JSON

## Usage

`npm install --save express-json-status-codes`

```
var express = require('express'),
    statusCodes = require('express-json-status-codes');

// Add the new responses to the `express.response` prototype
var extendedExpress = statusCodes(express);

var app = extendedExpress();
...

app.get('/', function(req, res) {
  res.ok('What's up');
});
```
