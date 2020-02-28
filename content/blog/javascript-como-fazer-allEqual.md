---
title: como usar o allEqual no javascript es6
date: "2020-01-04"
description: ''
tags: array,function,beginner
---

Check if all elements in an array are equal.

Use `Array.prototype.every()` to check if all the elements of the array are the same as the first one.
Elements in the array are compared using the strict comparison operator, which does not account for `NaN` self-inequality.

```js
const allEqual = arr => arr.every(val => val === arr[0]);
```

```js
allEqual([1, 2, 3, 4, 5, 6]); // false
allEqual([1, 1, 1, 1]); // true
```


[Acesse a Referência original](http://github.com/30-seconds/)
