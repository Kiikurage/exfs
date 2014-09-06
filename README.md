exfs
====
convenience extension of fs

## Install

```bash
npm install exfs
```


## usage

### original fs funcrions
This package has original functions in fs. So, you can use this package as below.

```Javascript
var fs = require("exfs");

//you can use fs as original usage.

```

### exfs.mkdir(path, [mode], callback, **createFlag**)
Asynchronously make directory if directory isn't exist

When the directory in which new folder will be made is not exist, if `createFlag=true`, this function make it. if `createFlag=false`, this function throw an error.

```Javascript
var fs = require("exfs");
fs.mkdir("./you/can/make/this/very/very/deep/directory/at/a/time", callback, true);
```

### exfs.writeFile(filename, data, [options], callback, **createFlag**)
Asynchronously writes data to a file

When the directory in which file is made is not exist, if `createFlag=true`, this function make it. if `createFlag=false`, this function throw an error.

```Javascript
var fs = require("exfs");
var path = ("./you/can/make/this/very/very/deep/directory/at/a/time");

fs.writeFile(path, "Hello World!", callback, true);
```
