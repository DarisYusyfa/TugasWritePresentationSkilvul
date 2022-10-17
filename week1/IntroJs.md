# Javascript 
adalah sebuah bahasa pemrograman yang digunakan untuk membuat sebuah website menjadi interaktif. Javascript memiliki 3 jenis yaitu, DOM, event, dan function.

## Variabel
Variabel adalah sebuah tempat untuk menyimpan sebuah nilai. Variabel memiliki 3 jenis yaitu, var, let, dan const. Var adalah sebuah variabel yang dapat digunakan untuk menyimpan sebuah nilai, let adalah sebuah variabel yang dapat digunakan untuk menyimpan sebuah nilai, dan const adalah sebuah variabel yang dapat digunakan untuk menyimpan sebuah nilai.
```js
var nama = "Daris yusyfa";
let nama = "Daris yusyfa";
const nama = "Daris yusyfa";
```
## Operator
Operator adalah sebuah simbol yang digunakan untuk melakukan operasi matematika. Operator memiliki 3 jenis yaitu, aritmatika, perbandingan, dan logika. Operator aritmatika adalah sebuah simbol yang digunakan untuk melakukan operasi matematika, operator perbandingan adalah sebuah simbol yang digunakan untuk melakukan operasi perbandingan, dan operator logika adalah sebuah simbol yang digunakan untuk melakukan operasi logika.

var a = 10;
var b = 5;
var c = a + b;
var d = a - b;
var e = a * b;
var f = a / b;
var g = a % b;
var h = a == b;
var i = a != b;
var j = a > b;
var k = a < b;
var l = a >= b;
var m = a <= b;
var n = a && b;
var o = a || b;
## Array
Array adalah sebuah variabel yang dapat digunakan untuk menyimpan banyak nilai. Array memiliki 3 jenis yaitu, array index, array length, dan array method. Array index adalah sebuah variabel yang dapat digunakan untuk menyimpan banyak nilai, array length adalah sebuah variabel yang dapat digunakan untuk menyimpan banyak nilai, dan array method adalah sebuah variabel yang dapat digunakan untuk menyimpan banyak nilai.
```js
var nama = ["Daris", "yusyfa"];
var nama = new Array("Daris", "yusyfa");
```
## Object
Object adalah sebuah variabel yang dapat digunakan untuk menyimpan banyak nilai. Object memiliki 3 jenis yaitu, object property, object method, dan object constructor. Object property adalah sebuah variabel yang dapat digunakan untuk menyimpan banyak nilai, object method adalah sebuah variabel yang dapat digunakan untuk menyimpan banyak nilai, dan object constructor adalah sebuah variabel yang dapat digunakan untuk menyimpan banyak nilai.
```js
var nama = {
	namaDepan: "Daris",
	namaBelakang: "yusyfa",
};
```
## Looping
Looping adalah sebuah perulangan yang digunakan untuk melakukan perulangan. Looping memiliki 3 jenis yaitu, for, while, dan do while. For adalah sebuah perulangan yang digunakan untuk melakukan perulangan, while adalah sebuah perulangan yang digunakan untuk melakukan perulangan, dan do while adalah sebuah perulangan yang digunakan untuk melakukan perulangan.
```js
for (var i = 0; i < 10; i++) {
	console.log(i);
}

// while loop
var i = 0;
while (i < 10) {
	console.log(i);
	i++;
}

// do while loop
var i = 0;
do {
	console.log(i);
	i++;
} while (i < 10);
```
## Conditional

Conditional adalah sebuah kondisi yang digunakan untuk menentukan sebuah kondisi. Conditional memiliki 3 jenis yaitu, if, else if, dan else. If adalah sebuah kondisi yang digunakan untuk menentukan sebuah kondisi, else if adalah sebuah kondisi yang digunakan untuk menentukan sebuah kondisi, dan else adalah sebuah kondisi yang digunakan untuk menentukan sebuah kondisi.
```js
var a = 10;
var b = 5;
if (a > b) {
	console.log("a lebih besar dari b");
} else if (a < b) {
	console.log("a lebih kecil dari b");
} else {
	console.log("a sama dengan b");
}
```
## Ternary Operator
Ternary Operator adalah sebuah operator yang digunakan untuk menentukan sebuah kondisi. Ternary Operator memiliki 3 jenis yaitu, if, else if, dan else. If adalah sebuah operator yang digunakan untuk menentukan sebuah kondisi, else if adalah sebuah operator yang digunakan untuk menentukan sebuah kondisi, dan else adalah sebuah operator yang digunakan untuk menentukan sebuah kondisi.
```js
var a = 10;
var b = 5;
var c = a > b ? "a lebih besar dari b" : "a lebih kecil dari b";
```
## Short Circuit
Short Circuit adalah sebuah kondisi yang digunakan untuk menentukan sebuah kondisi.
```js
var a = 10;
var b = 5;
var c = a > b && "a lebih besar dari b";

var d = a < b || "a lebih kecil dari b";
```
## Function
Function adalah sebuah fungsi yang digunakan untuk melakukan sebuah fungsi. Function memiliki 3 jenis yaitu, function declaration, function expression, dan arrow function. Function declaration adalah sebuah fungsi yang digunakan untuk melakukan sebuah fungsi, function expression adalah sebuah fungsi yang digunakan untuk melakukan sebuah fungsi, dan arrow function adalah sebuah fungsi yang digunakan untuk melakukan sebuah fungsi.
```js
function nama() {
	console.log("Daris Yusyfa");
}

var nama = function () {
	console.log("Daris Yusyfa");
};

var nama = () => {
	console.log("Daris Yusyfa");
};
```
## Scope
Scope adalah sebuah variabel yang digunakan untuk menentukan sebuah variabel. Scope memiliki 3 jenis yaitu, global scope, local scope, dan block scope. Global scope adalah sebuah variabel yang digunakan untuk menentukan sebuah variabel, local scope adalah sebuah variabel yang digunakan untuk menentukan sebuah variabel, dan block scope adalah sebuah variabel yang digunakan untuk menentukan sebuah variabel.
```js
var a = 10;
function nama() {
	var b = 5;
	console.log(a);
	console.log(b);
}
nama();
console.log(a);
console.log(b);
```
## Data Type Built-in Function
Data Type Built-in Function adalah sebuah fungsi yang digunakan untuk menentukan sebuah fungsi. Data Type Built-in Function memiliki 3 jenis yaitu, string, number, dan boolean. String adalah sebuah fungsi yang digunakan untuk menentukan sebuah fungsi, number adalah sebuah fungsi yang digunakan untuk menentukan sebuah fungsi, dan boolean adalah sebuah fungsi yang digunakan untuk menentukan sebuah fungsi.
```js
var a = "Daris Yusyfa";
var b = 10;
var c = true;
console.log(a.length);
console.log(b.toFixed(2));
console.log(c.toString());
```
## DOM
DOM adalah sebuah fungsi yang digunakan untuk menentukan sebuah fungsi. DOM memiliki 3 jenis yaitu, document, element, dan event. Document adalah sebuah fungsi yang digunakan untuk menentukan sebuah fungsi, element adalah sebuah fungsi yang digunakan untuk menentukan sebuah fungsi, dan event adalah sebuah fungsi yang digunakan untuk menentukan sebuah fungsi.
```js
var a = document.getElementById("nama");
var b = document.getElementsByTagName("p");
var c = document.getElementsByClassName("nama");
var d = document.querySelector("#nama");
var e = document.querySelectorAll(".nama");
var f = document.createElement("p");
var g = document.createTextNode("Daris Yusyfa");
var h = document.createAttribute("class");
```
## Event
Event adalah sebuah fungsi yang digunakan untuk menentukan sebuah fungsi. Event memiliki 3 jenis yaitu, event listener, event handler, dan event object. Event listener adalah sebuah fungsi yang digunakan untuk menentukan sebuah fungsi, event handler adalah sebuah fungsi yang digunakan untuk menentukan sebuah fungsi, dan event object adalah sebuah fungsi yang digunakan untuk menentukan sebuah fungsi.
```js
var a = document.getElementById("nama");
a.addEventListener("click", function () {
	console.log("Daris Yusyfa");
});
```

