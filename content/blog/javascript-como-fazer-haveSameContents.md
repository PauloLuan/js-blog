---
title: como usar o haveSameContents no javascript es6
date: "2020-01-04"
description: ''
tags: array,intermediate
---

Returns `true` if two arrays contain the same elements regardless of order, `false` otherwise.

Use a `for...of` loop over a `Set` created from the values of both arrays.
Use `Array.prototype.filter()` to compare the amount of occurences of each distinct value in both arrays.
Return `false` if the counts do not match for any element, `true` otherwise.

```js
const haveSameContents = (a, b) => {
  for (const v of new Set([...a, ...b]))
    if (a.filter(e => e === v).length !== b.filter(e => e === v).length) return false;
  return true;
};
```

```js
haveSameContents([1, 2, 4], [2, 4, 1]); // true
```

[Acesse a Referência original](http://github.com/30-seconds/)
