## Javascript Object

- Membuat sebuah object

  Sama seperti tipe data sebelumnya. Object dapat diassign kedalam sebuah variabel.

  contoh

  ```js
  let human = {
    name: 'Daris',
    age: '22',
    isVerified: true,
  }

  Sama seperti array, didalam object kita dapat menyimpan properti dengan tipe data apapun
  ```

## Mengakses Object dan Property nya

contoh

```js
let human = {
  name: 'Daris',
  age: '22',
  isVerified: true,
}
console.log(human);

//mengakses property object
contoh :

let human = {
  name: 'Daris',
  age: '22',
  isVerified: true,
}
console.log(person.name);
//output Daris


//menggunakan bracket notation
let human = {
  name: 'Daris',
  age: '22',
  'current address': 'Cianjur, jawabarat',
}
console.log(people['name']);// Daris

console.log(people['current address'])// 'Cianjur, jawabarat'
```

## Update dengan tipe data Obeject

Do's
Object dapat mengupdate value dari key yang sudah tersedia
Object dapat menambahkan key dan value baru

Dont's
Jika menggunakan constant pada variable object. Kita tidak bisa mengganti seluruh data object dengan object yang baru.

Jadi jika membutuhkan untuk update seluruh data object gunakan ‘let’ pada saat deklarasi variabel.

Contoh

```js
let human = {
  name: 'Daris',
  age: '22',
  isVerified: true,
};
human = {
  fullname: 'Daris',
};
console.log(human);
// output { fullname : 'Daris',}
```

## Delete Object Property

Kita dapat menghapus properti dari object menggunakan delete operator.

contoh

```js
let human = {
  name: 'Daris',
  age: '22',
  isVerified: true,
};
delete human.age;
console.log(human);
//output : name : Daris isVerified : true
```

## Method

Jika value yang kita masukkan pada property berupa function.

Maka itu disebut method.
log() adalah property yang berupa function dari object console.

Sehingga kita memanggila dengan cara console.log().

contoh

```js
const meeting = {
  welcome: function () {
    return 'Hai selamat bergabung';
  },
  afterTransaction: function () {
    return 'Terimakasih sudah mau bergabung';
  },
};

console.log(meeting.welcome()); // Terimakasih sudah mau bergabung
```

## Nested Object
