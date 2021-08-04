# Functions in JavaScript

---

## 1) Behaviour of Function -

- Function can be overwritten.
- Function can get Hoisted
- Function acts like a container.
- Function has local and global scope.
- First Class Citizen.
- Function returns a reference.
- Function can return another Function.
- Object

## 2) Function Declaration and Calling

#### 2.1 Setting up the Function

```javascript
function car() {
  console.log("BMW");
}
car(); // CALLING A FUNCTION CAR

output: BMW;
```

#### 2.2 Passing parameter to the Function

- We can also pass parameter to the function.

```javascript
function favfood(fruit) {
  console.log("favFood is ", fruit);
}

var fruit = "orange"; // passing orange as parameter
favfood(fruit); // calling the function

output:
favFood is orange
```

#### 2.3 Saftey Net or Safety Check

!! fn_name && (typeof fn_name === "function")&& fn_name()

- This checks whether it is really a function or not if it is a function then it executes it.

```javascript
function sport(val) {
  !!sport && typeof sport === "function" && sport(val);
  console.log("favSports is ", val);
}
var val = "football";
sport(val);

output:
favSport is football
```

## 3) Different ways to Declare a Function

- There are two ways you can declare a functions.
  - Function Declaration
  - Function Assignment

#### 7.3.1) Function Declaration

```javascript
function fn_name() {
  console.log("hello");
}
fn_name();
```

#### 7.3.2) Function Assignment

```javascript
var fn_name2 = function () {
  console.log("bye bye!");
};

fn_name();
```

## 4) Function Returning a Function

- A function can also return another function with the help of "return".

Example:

```javascript
function hello(a) {
  console.log("1." a);

  function hello2(){
    console.log("2.", a * 2)
  }
  return hello2; // returning th function hello2
}

var val = 20;
var result = hello(val) // hello2 referene is stored in result
result(); // calling result() but result has reference of hello2 so hello2 is called.

output-
1.  20
2.  40
```

## 5) Function Passed As a Parameter

- A function can also be passed a parameter.

Example:

```javascript
const print = function (value) {
  console.log("printing", value);
};

const completeTask = function (b) {
  const a = "200";
  const c = a * 5;
  b(c);
};
var final = completeTask(print); //Here we are passing print function as a parameter to the completeTask function. "b" is holding the reference to print function
console.log(final);
```

## 6) Higher Order Function

- Higher Order function means any Function which takes Function as a parameter or returns a Function is called Higher order funtion.
- We use it to make our code more flexible or rohbust.

Example:

```javascript
var sport = function () {
  var cricket = function (player) {
    var IPL = function (team) {
      return team;
    };
    return IPL;
  };
  return cricket;
};

var localsport = sport(); // Reference of cricket function is stored in localsport
var result = localsport("ABD");
// cricket function has passed a parameter & Reference of IPL function is stored in result
var final = result("Mumbai Indians");
// IPL function has passed a parameter & Reference of IPL function is stored in result

console.log(final);
// Calling IPL function

output: Mumbai Indians
```

### 6.1) Short-Circuit OR CastCading

- It is used to write the code in shorter format.

Example:

```javascript
var sport = function () {
  var cricket = function (player) {
    var IPL = function (team) {
      return team;
    };
    return IPL;
  };
  return cricket;
};

var res = sport()("ABD")("Mumbai Indians"); // short-circuit  / Castcading
```

### 6.3) CLOSURE

- In javaScript whenever you define a function under a function so the scope of the function is only limited to that function. Which is called as "CLOSURE".

```javascript
function fn_name() {
  console.log("20");
}

function main() {
  function outside() {
    console.log("from inside");
    fn_name();
  }
  console.log("from outside");
  fn_name();
  output();
}
main();

output:
from inside
20
from outside
20
```

## 7) Pure Function

- In pure function we do not update,modify,change,overwrite the parameter value.

Example:

```javascript
function add(a, b) {
  return a + b; // if change the value of a over here then it would not be  called a pure funtion
}
add(10, 20);
```

## 8) IIFE (Immediately Invoke Function Expression)

- IIFE functions can only be called once because they don't have a variable or name attached to them
- It is invoked as soon as it is declared.
- To safeguard our code we use semi-colon (;) at the start.

Example:

```javascript
;(function () {
  console.log("Initialization...");
})();

output: Initialization..
```

## 9) Arrow Function

- Arrow function is newly added feature of ES6.
- It is basically a shortcut method to write a function.

```javascript
// normal way
var b = function () {
  console.log("hello");
};

// Arrow function
var b = () => {
  console.log("hello from arrow function");
};
```
