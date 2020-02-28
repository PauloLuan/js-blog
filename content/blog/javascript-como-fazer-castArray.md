---
title: como usar o castArray no javascript es6
date: "2020-01-04"
description: ''
tags: utility,array,type,beginner
---

Casts the provided value as an array if it's not one.

Use `Array.prototype.isArray()` to determine if `val` is an array and return it as-is or encapsulated in an array accordingly.

```js
const castArray = val => (Array.isArray(val) ? val : [val]);
```

```js
castArray('foo'); // ['foo']
castArray([1]); // [1]
```


[Acesse a Referência original](http://github.com/30-seconds/)
