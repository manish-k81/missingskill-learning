# Built In JavaScript Functions

---

1. SetTimeout - It is executed after some time.

```javascript
setTimeout(function () {
  console.log("I am Running..");
}, 2000);

// It will executed after 2 secs
```

2. SetInterval - It runs continuosly after 2 secs it doesn't stop.

```javascript
setInterval(funtion(){
  console.log ("i will not stop");
},2000)
```

3. ParseInt - It converts the input into a integer.It removes the decimal point.

- It is very RISKY to use.

```javascript
const num = 10.12;
let intnum = ParseInt(num);
console.log(intnum);
```

4. ParseFloat - It coverts a string and returns a floating point number.

```javascript
const a = Man34nish.92
let res = a.pareseFloat(a) // 34.92
```

5. JSON

| Built in       | Description                                |
| -------------- | ------------------------------------------ |
| JSON.stringify | Converts object into JSON data             |
| JSON.parse     | Converts JSON data into JavaScript objects |
