# WEB STORAGE

web storage sama hal nya seperti cookies atau lainnya jadi kita bisa menyimpan data yang kita punya kedalam pemyimpanan web seperti cookies

contoh

```js
<!DOCTYPE html>
<html lang="en">
 <head>
   <meta charset="UTF-8" />
   <meta http-equiv="X-UA-Compatible" content="IE=edge" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
   <title>Todo List</title>
   <link rel="stylesheet" href="style.css" />
 </head>
 <body class="">
   <form action="" class="container">
     <input type="text" placeholder="Hari ini saya akan..." />
     <ul id="list-container"></ul>
   </form>
   <button id="toggle">Toggle</button>

   <script src="script.js"></script>
 </body>
</html>
```

.js

```js
// ==================== init penampung list dari todo
const todos = [];

// ==================== check ketika pertama kali website di buka, apakah ada key: theme dan value: dark di storage
if (localStorage.getItem('todo')) {
  const todoStore = JSON.parse(localStorage.getItem('todo'));

  todoStore.map((todo) => {
    const li = document.createElement('li');
    li.innerText = todo;

    const container = document.querySelector('#list-container');
    return container.appendChild(li);
  });
}

// ==================== check ketika pertama kali website di buka, apakah ada key: theme dan value: dark di storage
document.querySelector('form').addEventListener('submit', (ev) => {
  ev.preventDefault();
  const userInput = document.querySelector('input').value;

  const li = document.createElement('li');
  li.innerText = userInput;

  todos.push(userInput);

  localStorage.setItem('todo', JSON.stringify(todos));

  const container = document.querySelector('#list-container');
  container.appendChild(li);
});

/* 
  Conclucion:
  JSON.parse -> ubah string ke object 
  JSON.stringify -> ubah apapun ke string JSON
*/
```

css

```css
@import 'https://fonts.googleapis.com/css?family=Poppins';

/*
  hint untuk dark-theme
  :root 
  var()  
  bisa cek folder dark-mode
*/

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  background: #e0e0e0;
  min-height: 100vh;
  font-family: 'Poppins', Arial, Helvetica, sans-serif;
}

body.dark {
  background: black;
  color: white;
}

.container {
  padding-top: 50px;
  max-width: 500px;
  margin: auto;
}

input {
  width: 100%;
  padding: 5px 8px;
  border: 1px solid rgb(121, 121, 121);
  border-radius: 8px;
}

#list-container li {
  margin: 10px 0;
  padding: 8px 12px;
  list-style: none;
  background: #e0e0e0;
  border: 1px solid rgb(180, 180, 180);
  border-radius: 8px;
  box-shadow: 23px 23px 46px #d0d0d0, -23px -23px 46px #f0f0f0;
}
```
