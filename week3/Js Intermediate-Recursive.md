```js
//Function recursive punya
// base case -> titik paling kecil(berhenti)
// recursion case -> titik dia manggil diri dia sendiri

// ====================================================
// menampilkan deret angka 1 2 3 4 5
// cari solusi paling kecil

// 1
// 1 2
function deretAngka(n){
  if (n == 1) {
    console.log(n)
  } else {
    deretAngka(n-1)
    console.log(n);
  }
}
// deretAngka(7)

// ==================================================
// mencari angka faktorial
// 5!
// 5 x 4 x 3 x 2 x 1

// cari solusi paling kecil
// 1! -> 1
// 2! -> 2 x 1
function faktorial(n) {
  if (n == 1) {
    return 1
  } else {
    return n * faktorial(n - 1)
  }
}
console.log(faktorial(5))

// loop vs revursive
function faktorialFor(n) {
  let hasil = 1
  for (let i = n; i >= 1; i--){
    hasil = hasil * i
    console.log(i)
  }
  return hasil
}
console.log(faktorialFor(3));
```

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>
</head>
<body>
  
  <script src="./script.js"></script>
</body>
</html>
```