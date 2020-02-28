---
title: como usar o without no javascript es6
date: "2020-01-04"
description: ''
tags: array,beginner
---

Filters out the elements of an array, that have one of the specified values.

Use `Array.prototype.filter()` to create an array excluding(using `!Array.includes()`) all given values.

```js
const without = (arr, ...args) => arr.filter(v => !args.includes(v));
```

```js
without([2, 1, 2, 3], 1, 2); // [3]
```


[Acesse a Referência original](http://github.com/30-seconds/)
