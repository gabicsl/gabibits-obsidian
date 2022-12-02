**Linguagem**:: #JavaScript 
**Links**:: https://www.30secondsofcode.org/articles/s/js-remove-array-duplicates

---


# Código
```js
const nums = [1, 2, 2, 3, 1, 2, 4, 5, 4, 2, 6];

[...new Set(nums)] // [1, 2, 3, 4, 5, 6]
```