# Some ES6 Functions

---

1. **Object.assign**

- It creates a new memory location and copies all the primitive datatypes. Now if we change something in user the user2 does not changes.

```javascript
let user = { tags: ["manish", "Raj", "Joy"], index: 10 };

let user2 = user.object.assign({}, user);
```

2. **Spread Operator**

- It is used for Non-Primitive Datatypes. It splits the element of array in its individual
  component.

```javascript
var people = ["manish", "raj", "vegeta"];
console.log(...people);

output:
manish raj vegeta
```

3. Rest Operator

- The rest is used to store the keys which are not plucked individually.

Example:

```javascript
let user = {
  "id":10,
  "isActive":Flase,
  "age":21,
  "friends":[
    {
      "id":0,
      "name":manish
    },
    {
      "id": 1,
      "name": pulkit
    }
  ]
}

let {id,age,isActive, ...rest} = user;
console.log("1.", rest , "" , "2.", user);

output:
1.
"friends":[
    {
      "id":0,
      "name":manish
    },
    {
      "id": 1,
      "name": pulkit
    }
  ]
2.
{
  "id":10,
  "isActive":Flase,
  "age":21,
}
```

## 2. Destructuring

3.1) For Objects

```javascript
var user = {
  id: 10,
  age: 21,
  name: "manish",
};

let { id, age, name } = user; // Destructuring
```

3.2) For Arrays

```javascript
let tags = ["orange", "mango", "apples"];

let [first, second, third] = tags;
```
