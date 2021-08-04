# Objects

---

## 1. Object Creations

- Objects are denoted by using "{}" curly braces

- Objects are always in the form of pair which looks like this key:values

```javascript
var user {
  id: 10,
  name: "manish",
  age: 21,
};
user.movie = "inception"
```

## 2. Differnet Ways To Create An Object

---

- There are 3 ways in which you can create a object.

  - var a = {}
  - var a = new Object();
  - Object.create()

## 3. Built In Methods Of Object

---

| Method | How to write        | Description                                                   |
| ------ | ------------------- | ------------------------------------------------------------- |
| value  | Object.value(user)  | Fetches all the values of the user object                     |
| key    | Object.keys(user)   | Fetches all the keys of the user object                       |
| freeze | Object.freeze(user) | It is used to stop the changes which are adding to the object |

# 4. Object Prototype and Constructor

---

- In JavaScript we do not have "OOPS" so to mimic "OOPS" Javascript introduced object prototype. Where function is converted into object prototype.

- The **new** keyword is used to create the instance on the object. A constructor is called when an object is declared by using the new keyword.

- The use of **(this)** keyword is used to access the properties of a particular function.

Example:

```javascript
function person(username, age) { // this becomes a class
  this.username = username; // here this keyword refers to person function
  this.age = age;
}
var result = new person("Manish", "21"); // instance of an object is created
//it becomes object constructor

console.log("1."result);
console.log("2."result.username);

output:
 1. person{
  username : Manish
  age :21
}
2. Manish
```

- The moment we add new keyword "var result" becomes the Object Constructor and function person becomes a Class or Prototype Object.

- Constructor Functions are not really favoured to use.

**NOTE -**

- In JavaScript whenever we define a function inside a Object it is refered as **"METHOD"**.

Example:

```javascript
user = {
  index: 10,
  age: 21,

  getIndex: function () {
    // This is known as a METHOD
    return user.index;
  },
};
```
