---
title: como usar o maxDate no javascript es6
date: "2020-01-04"
description: ''
tags: date,math,beginner
---

Returns the maximum of the given dates.

Use the ES6 spread syntax with `Math.max` to find the maximum date value, `new Date()` to convert it to a `Date` object.

```js
const maxDate = dates => new Date(Math.max(...dates));
```

```js
const array = [
  new Date(2017, 4, 13),
  new Date(2018, 2, 12),
  new Date(2016, 0, 10),
  new Date(2016, 0, 9)
];
maxDate(array); // 2018-03-11T22:00:00.000Z
```


[Acesse a Referência original](http://github.com/30-seconds/)
