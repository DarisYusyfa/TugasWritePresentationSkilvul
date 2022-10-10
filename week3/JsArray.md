# ARRAY

Array adalah tipe data OL yang bisa menyimpan tipe data apapun dalam jumlah banyak
array bisa menyimpan tipe data string number boolean dll

contoh

```js
const handPhone = ['Iphone', 'Samung', 'Xiomi', 'Huawei', 'Vivo'];
console.log(handPhone);

//menyimpan banyak tipe data

let random = ['Malboro', '30', 'true'];
console.log(random);
```

## Cara Membuat Array

Pertama menggunakan square bracket,array juga dihitung dari index data 0
dan data pertama adalah index 01234 dst

## Update Array

kita juuga bisa megubah,menambah array tsb

contoh

```js
let handPhone = ['Iphone', 'Samung', 'Xiomi', 'Huawei', 'Vivo'];

handPhone[0] = 'Oppo';
console.log(handPhone);
//dari kode diatas maka akan dapat kesimpulam nama hp iphone akan berunah menjadi nama oppo
```

## Const Array

jika menggunakan variable const kita tidak bisa mengupdate data ,akan tetapi itu tidak berlaku pada array dan const ini hanya bisa mengupdate konten nilai dalam array

contoh

```js
const buah = ['appel', 'sirsak', 'mangga', 'jeruk'];

buah = ['semangka'];
console.log(buah);
//output error
```

akan tetapi jika menggunakan contoh dibawah ini

```js
const buah = ['appel', 'sirsak', 'mangga', 'jeruk'];

buah[3] = ['nanas'];
//output appel sirsak mangga nanas , si jeruk nya diganti dengan nanas
```

## Array Properties

array memiliki constructor,lenth,index,input,dan prototype

contoh array length

```js
let handPhone = ['Iphone', 'Samung', 'Xiomi', 'Huawei', 'Vivo'];
console.log(handPhone.length);
//otput 5
```

## Array Method

Kita tidak perlu membuat function lagi jika method yang kita butuhkan sudah tersedia.

contoh

```js
let handPhone = ['Iphone', 'Samung', 'Xiomi', 'Huawei', 'Vivo'];

handPhone.push(Oppo);
//output Iphone,Samsung,Xiomi,Huawei,Vivo,Oppo
.push adalah untuk menambahkan array


let handPhone = ['Iphone', 'Samung', 'Xiomi', 'Huawei', 'Vivo'];

handPhone.pop();
console.log(handPhone)
// .pop untuk menghapus
// .unshift untuk menambahkan item pada index pertama
// .sort untuk mengurutkan secara ascending atau descending
```

## Looping pada Array

untuk melooping kita bisa menggunakan .map() dan .forEach()

```js
//contoh .forEach()
const buah = ['appel', 'sirsak', 'mangga', 'jeruk'];
buah.forEach(element =>{
  console.log(buah)
});
//output appel,sirsak,mangga,jeruk


//contoh .map()
let arr = [1,2,3,4,5];

let doubled = arr.map(num=>{
  return num * 2;
});
console.log(doubled);
//Perbedaannya adalah .forEach tidak dapat membuat Array baru dari hasil operasi yang ada dalam looping

Lalu dari segi performance juga sangat jauh.
adi, gunakan .forEach() jika hanya memerlukan looping untuk menampilkan saja atau menyimpan ke database.

Gunakan .map() jika akan melakukan operasi pada array seperti yang dapat mengubah nilai array sebelumnya.
```
