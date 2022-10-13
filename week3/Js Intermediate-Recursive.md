# Recursive Function

Recursive function adalah fungsi yang memanggil dirinya sendiri.

```js
Contoh Recursive Function
function factorial(n) {
  if (n === 0) {
    return 1;
  } else {
    return n * factorial(n - 1);
  }
}

console.log(factorial(5));
```
