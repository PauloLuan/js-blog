---
title: como usar o filterNonUnique no javascript es6
date: "2020-01-04"
description: ''
tags: array,beginner
---

Filters out the non-unique values in an array.

Use `Array.prototype.filter()` for an array containing only the unique values.

```js
const filterNonUnique = arr => arr.filter(i => arr.indexOf(i) === arr.lastIndexOf(i));
```

```js
filterNonUnique([1, 2, 2, 3, 4, 4, 5]); // [1, 3, 5]
```


[Acesse a Referência original](http://github.com/30-seconds/)
