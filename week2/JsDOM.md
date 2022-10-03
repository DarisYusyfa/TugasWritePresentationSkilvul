# DOM

Dom singkatan dari Document Object Model,Jadi, ketika halaman website kita diload, browser kita akan membuat Document Object Model dari halaman website dan strukturnya

Dom juga bukan bagian dari javascript melainkan browser web API

## Memamanipulasi Element HTML

- Mencari element HTML

contoh

```js
//Mencari 1 element dengan id
document.getElementById('header');

//Mencari beberapa element sekaligus
document.getElementsByClassName('container');

//Mencari element menggunakanselector sperti getElementsByClassName
document.querrySelector('*header p span');
```

catatan : Perlu dijelasin kalau getElementsByClassName itu bakal ngereturn bentuk array; walaupun cuma ada 1 element dengan class itu
Kalau bisa diulangin lagi penggunaan id dan class (id cuma boleh 1 element per page, class bisa beberapa sekaligus dan per element bisa beberapa class

- Mengubah konten Element

Element.textContent

contoh

```js
<h1 id="heading"></h1>;

document.getElementById('heading').textContent = 'Text Heading';
```

sama seperti menulis

```js
<h1 id ='heading'>Teks heading</h1
```

Element.innerHTML

contoh

```js
const heading = document.createElement('h1');
heading.textContent = 'Ini Heading';

document.getElementById('header').appendChild(heading);
```

sama sperti menulis

```js
<div id="header">
<h1>ini heading</h1>

// .createElement() ->.textContent untuk mengubah kontennya -> .appendChild() untuk menambahkan ke DOM
```

Ada beberapa jenis Interaksi menggunakan HTML DOM Event yaitu
click,focus,change,hover,blur,submit,scroll

- Interaksi User

Element.addEventListener("event")

-Bisa dihilangkan
-Menampung beberapa event listener untuk 1 element
-Memiliki argument tambahan

EventListener-click
contoh

```js
<iput id="user-input"/><button id="alert-button">ini button</button>

const input = document.getElementById("user-input")
const button = document.getElementById("alert-button")

//dan tambahkan event listener

button.addEventListener("click", function(){
  alert(input.value)
})
```
