# TypeData

Ada beberapa jenis type data di jsvascript antara lain Null,Undifined,Boolean,Number,String,Symbol,NaN,Object,Array

## String

adalah tipe data JavaScript yang menyimpan informasi dalam teks. String dikemas dengan tanda kutip (tidak seperti angka, yang tidak membutuhkannya). Tanda kutip ganda dan tunggal diterima, tetapi hati-hati dan jangan mencampur keduanya dalam satu string

contoh penulisan string

```js
const nama = 'Daris'; // double quote
var kelas = 'IPA 1'; // single quote
```

## Number

Number pada JavaScript dapat ditulis dengan atau tanpa desimal,Number tidak boleh ditulis dalam tanda kutip, jika tidak, itu akan dibaca sebagai string

contoh penulisan Number

```js
var angka = 20; // tanpa bilangan desimal
const number = 2.0; // dengan bilangan desimal
```

## Math

Math atau Object Math Sama seperti objek pada umumnya, objek Math memiliki properti, nilai, dan method.

Objek Math hanya bisa digunakan untuk tipe data number, dan tidak bisa digunakan untuk tipe data BigInt

contoh

```js
let result = Math.sqrt(9); // Output: 3

let result = Math.sqrt(BigInt(9)); // Output: TypeError: Cannot convert a BigInt value to a number
```

Keuntungan memakai objek Math adalah kita tidak perlu lagi mikir dalam menulis kode ketika membuat operasi Matematika.

## Type Data Primitive dan Non Primitive

Tipe data adalah jenis data yang dapat disimpan, dimanipulasi, dan digunakan untuk memberi tahu komputer bagaimana menfasirkan nilai atau datanya.

primitive terdiri dari string,number,BigInt,Boolean,Undefined,Null,Symbol

Non Primitive Yaitu Object dan Array

- Primitive

  Tipe data primitif hanya dapat menyimpan satu nilai pada satu waktu dan tidak dapat diubah menggunakan cara yang sama seperti tipe data non-primitif. Tipe data Primitif akan dianggap sama jika nilainya sama.

  contoh

  ```js
  //primitif tidak dapat diubah
  const nama = 'Daris';
  console.log(nama[0]); //D
  ```

- Non Primitive

  Tipe data non-primitif dapat menyimpan lebih dari satu nilai pada satu waktu dan dapat diubah. Tipe data non-primitif akan dianggap berbeda meskipun nilainya sama dan dalam urutan yang sama.

  contoh

  ```js
  ///NonPrimitif dapat diubah
  const mahasiswa = ['daris', 'yusyfa', 'atqia'];
  mahasiswa[0] = 'muhammad';
  console.log(mahasiswa); //['muhammad', 'yusyfa', 'atqia']
  ```
