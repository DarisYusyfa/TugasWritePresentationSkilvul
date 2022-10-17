# Asycnhronous JavaScript
  Asynchronous JavaScript adalah JavaScript yang dapat melakukan proses secara paralel. Asynchronous JavaScript menggunakan callback function untuk menangani proses yang dilakukan secara asynchronous.

## Contoh Asynchronous JavaScript
  ```js
  console.log("Start");

  setTimeout(() => {
    console.log("Callback function fired");
  }, 2000);

  console.log("End");
  ```
## Contoh Asynchronous JavaScript dengan Callback
  ```js
  console.log("Start");

  function getUser(id, callback) {
    setTimeout(() => {
      console.log("Reading a user from a database...");
      callback({ id: id, gitHubUsername: "daris" });
    }, 2000);
  }

  function getRepositories(username, callback) {
    setTimeout(() => {
      console.log("Calling GitHub API...");
      callback(["repo1", "repo2", "repo3"]);
    }, 2000);
  }

  getUser(1, (user) => {
    console.log("User", user);
    getRepositories(user.gitHubUsername, (repos) => {
      console.log("Repos", repos);
    });
  });

  console.log("End");
  ```
## Promise
  Promise adalah sebuah objek yang merepresentasikan keberhasilan atau kegagalan sebuah event yang asynchronous di masa yang akan datang. Promise memiliki 3 state, yaitu pending, fulfilled, dan rejected. Promise juga memiliki 2 callback, yaitu resolve dan reject. Resolve digunakan untuk mengubah state dari pending menjadi fulfilled. Reject digunakan untuk mengubah state dari pending menjadi rejected. Promise juga memiliki method, yaitu then dan catch. Then digunakan untuk menangani state fulfilled. Catch digunakan untuk menangani state rejected.
  ```js
  Contoh Promise
  const p = new Promise((resolve, reject) => {
    setTimeout(() => {
      resolve(1);
      reject(new Error("message"));
    }, 2000);
  });

  p.then((result) => console.log("Result", result)).catch((err) =>
    console.log("Error", err.message)
  );
  ```
  ```js
  Contoh Promise dengan Asynchronous JavaScript
  console.log("Start");

  function getUser(id) {
    return new Promise((resolve, reject) => {
      setTimeout(() => {
        console.log("Reading a user from a database...");
        resolve({ id: id, gitHubUsername: "daris" });
      }, 2000);
    });
  }

  function getRepositories(username) {
    return new Promise((resolve, reject) => {
      setTimeout(() => {
        console.log("Calling GitHub API...");
        resolve(["repo1", "repo2", "repo3"]);
      }, 2000);
    });
  }

  getUser(1)
    .then((user) => getRepositories(user.gitHubUsername))
    .then((repos) => console.log("Repos", repos))
    .catch((err) => console.log("Error", err.message));

  console.log("End");
  ```
## Async and Await
  Async dan await adalah cara untuk menangani proses asynchronous dengan cara yang lebih mudah. Async digunakan untuk membuat function menjadi asynchronous. Await digunakan untuk menunggu proses asynchronous selesai. Await hanya dapat digunakan di dalam function yang memiliki async. Await hanya dapat digunakan untuk menangani promise.

### Contoh Async and Await
  ```js
  console.log("Start");

  function getUser(id) {
    return new Promise((resolve, reject) => {
      setTimeout(() => {
        console.log("Reading a user from a database...");
        resolve({ id: id, gitHubUsername: "daris" });
      }, 2000);
    });
  }

  function getRepositories(username) {
    return new Promise((resolve, reject) => {
      setTimeout(() => {
        console.log("Calling GitHub API...");
        resolve(["repo1", "repo2", "repo3"]);
      }, 2000);
    });
  }

  async function displayRepositories() {
    try {
      const user = await getUser(1);
      const repos = await getRepositories(user.gitHubUsername);
      console.log("Repos", repos);
    } catch (err) {
      console.log("Error", err.message);
    }
  }

  displayRepositories();

  console.log("End");
  ```
## Fetch API
  Fetch API adalah API yang digunakan untuk mengambil data dari server. Fetch API menggunakan promise. Fetch API memiliki 2 method, yaitu GET dan POST. Method GET digunakan untuk mengambil data dari server. Method POST digunakan untuk mengirim data ke server.
  ```js
  Contoh Fetch API
  fetch("https://jsonplaceholder.typicode.com/posts")
    .then((response) => response.json())
    .then((json) => console.log(json));
  Contoh Fetch API dengan Async and Await
  async function displayPosts() {
    const response = await fetch("https://jsonplaceholder.typicode.com/posts");
    const json = await response.json();
    console.log(json);
  }

  displayPosts();
  ```
  
