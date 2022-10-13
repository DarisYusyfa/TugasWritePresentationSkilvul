# Asynchronous

JavaScript async adalah JavaScript yang dapat melakukan proses secara paralel. Asynchronous JavaScript menggunakan callback function untuk menangani proses yang dilakukan secara asynchronous.

```js
Contoh Asynchronous JavaScript
console.log("Start");

setTimeout(() => {
  console.log("Callback function fired");
}, 2000);

console.log("End");
Contoh Asynchronous JavaScript dengan Callback
console.log("Start");

function getUser(id, callback) {
  setTimeout(() => {
    console.log("Reading a user from a database...");
    callback({ id: id, gitHubUsername: "ersankarimi" });
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

# Promise

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
Contoh Promise dengan Asynchronous JavaScript
console.log("Start");

function getUser(id) {
  return new Promise((resolve, reject) => {
    setTimeout(() => {
      console.log("Reading a user from a database...");
      resolve({ id: id, gitHubUsername: "ersankarimi" });
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
