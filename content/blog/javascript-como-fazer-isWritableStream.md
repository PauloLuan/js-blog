---
title: como usar o isWritableStream no javascript es6
date: "2020-01-04"
description: ''
tags: node,type,intermediate
---

Checks if the given argument is a writable stream.

Check if the value is different from `null`, use `typeof` to check if the value is of type `object` and the `pipe` property is of type `function`.
Additionally check if the `typeof` the `_write` and `_writableState` properties are `function` and `object` respectively.

```js
const isWritableStream = val =>
  val !== null &&
  typeof val === 'object' &&
  typeof val.pipe === 'function' &&
  typeof val._write === 'function' &&
  typeof val._writableState === 'object';
```

```js
const fs = require('fs');
isWritableStream(fs.createWriteStream('test.txt')); // true
```


[Acesse a Referência original](http://github.com/30-seconds/)
