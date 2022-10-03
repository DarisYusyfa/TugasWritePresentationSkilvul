# JAVASCRIPT SCOPE

- Block Scope

  Code yang berada pada kurung kurawal {} yang seeering digunakan pada Conditional,function dan Looping

- Global Scope

  Variable yang bisa diakses dimanapun dan varable itu harus dideklarasikan diluar block

  contoh :

  ```js
  let myLeader = 'Skilvul';

  function meeting() {
    return myLeader;
  }

  Console.log(myLeader);

  //Variable myLeader deklarasi secara g Scope
  ```

- Local Scope

  Mendeklarasikan variable dalam block yaitu hanya bisa di akses di dalam block saja seperti di dalam function, Conditional dan Looping

  ```js
  //declarsi variable dalam block function

  function meeting(){
      let myName = "Skilvul"
      return myLeader;
  }
  console.log(meeting())
  console.log(myName);

  pendeklarasian variable secara local Scope
  ```

# JS FUNCTION

Function yaitu sebuah blok kode untuk memudahkan kita saat menyelesaikan task dan bisa menggunakan kembali saat dibutuhkan

contoh function

```js
function meeting() {
  return 'Selamat siang';
}
// adapun cara memanggil funtion dengan cara seperti berikut

meeting();
console.log(meeting());
```

## Parameter dan argument

Prameter yaitu untuk menerima sebuah inputan data dari function dan biassanya digunakan untuk melakukan task/tugas

contoh parameter

```js
function perkalian(a, b) {
  return a * b;
}
```

Argument adalah nilai yang digunakan saat memanggil funtion, jumlah argument harus sama dengan jumlah parameternya
jadi ketika function mempunyai 4 nilai parameter maka kita gunakan 4 argument

conrtoh parameter dan argument

```js
function perkalian(a, b) {
  return a * b;
}
console.log(perkalian(5, 2)); // 10
```

Function sangat dubutuhkan untuk memanage code jika ada eror

Default paramaters digunakan untuk memberikan nilai awal/default pada parameter function.

Default parameters bisa digunakan jika kita ingin menjaga function agar tidak error saat dipanggil tanpa argumen

contoh default paramaters

```js
function greetOnWebsite(name = 'Stranger') {
  return 'Hello' + name;
}
console.log(greetOnWebsite('David')); // 'Hello David'
console.log(greetOnWebsite()); // 'Hello Stranger'
```

## Arrow Function

Arrow function yaitu cara lain untuk menuliskan function

contoh arrow function

```js
const meeting = () => {
    return 'Hai Saya Daris'
};

const perkalian = (2, 5) => {
    return 2 * 5;
};
```
