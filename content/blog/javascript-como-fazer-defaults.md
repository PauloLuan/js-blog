---
title: como usar o defaults no javascript es6
date: "2020-01-04"
description: ''
tags: object,intermediate
---

Assigns default values for all properties in an object that are `undefined`.

Use `Object.assign()` to create a new empty object and copy the original one to maintain key order, use `Array.prototype.reverse()` and the spread operator `...` to combine the default values from left to right, finally use `obj` again to overwrite properties that originally had a value.

```js
const defaults = (obj, ...defs) => Object.assign({}, obj, ...defs.reverse(), obj);
```

```js
defaults({ a: 1 }, { b: 2 }, { b: 6 }, { a: 3 }); // { a: 1, b: 2 }
```


[Acesse a Referência original](http://github.com/30-seconds/)
