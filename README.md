json-format
==========

Change for using with npm modules. [original version](https://github.com/phoboslab/json-format).

#### Instaling ####
```
  npm install json-format
```

#### Usage ###
```
  var jsonFormat = require('./');
  var fs = require('fs');
  var obj = {
    a: 1,
    b: 2
  }

  fs.writeFile('example.json', jsonFormat(obj), function(err){
    if (err) throw err;
    console.log('saved');
  });
```

#### Result ####
```
{
  "a": 1,
  "b": 2
}
```