---
title: como usar o is no javascript es6
date: "2020-01-04"
description: 'teste'
tags: type,array,regexp,beginner
---

Checks if the provided value is of the specified type.

Ensure the value is not `undefined` or `null` using `Array.prototype.includes()`, and compare the `constructor` property on the value with `type` to check if the provided value is of the specified `type`.

```js
const is = (type, val) => ![, null].includes(val) && val.constructor === type;
```

```js
is(Array, [1]); // true
is(ArrayBuffer, new ArrayBuffer()); // true
is(Map, new Map()); // true
is(RegExp, /./g); // true
is(Set, new Set()); // true
is(WeakMap, new WeakMap()); // true
is(WeakSet, new WeakSet()); // true
is(String, ''); // true
is(String, new String('')); // true
is(Number, 1); // true
is(Number, new Number(1)); // true
is(Boolean, true); // true
is(Boolean, new Boolean(true)); // true
```


[Acesse a Referência original](http://github.com/30-seconds/)
