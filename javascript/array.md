# ARRAY

---

- Array is nothing but a specialized object.

- Array is denoted by using "[]" square brackets.

```javascript
var array = ["goku", "vegeta", "naruto", "kakashi"];

console.log(array);
console.log(array[1]);

output: Array[4];
vegeta;
```

## 2) Methods of Array

```javascript
var names = ["manish", "raj", "vegeta", "goku"];
```

1. **Push Method.**

- Adds the name at the ending of the array.

```javascript
let val = names.push("simran"); // simran name is added at the end
```

2. **Pop Method**

- Removes an element from the array.

```javascript
let val = names.pop(); // last value is removed from array
```

3. **Unshift Method**

- It adds element at the beginning of the
  names.unshift("king"); // adds element at the beginning of the aaray

```javascript
let val = names.unshift(); // removes element from the beginning
```

4. **Concat**

- It is used for merging of two arrays.

```javascript
let val = names.concat(names2); // it is used for merging two arrays
```

5. **indexOf**

- It finds the index number of a particular element

```javascript
names.indexof("vegeta");
// finds the index number of vegeta
```

6. **Includes**

- It checks whether the given element is present in the array or not.

```javascript
let val = names.includes("raj");
// checks whether the element is present in array or not
```

7. **Slice**

- It splits the array in whichever input number we pass.

```javascript
names.slice(0, 2);
// splits the array\
```

8. **Array.isArray**

- Checks whether it is an array or not.

```javascript
let val = Array.isArray(names);
// checks whether its a array or not
```

## 3) Built in Methods Of Array

1.) **FOREACH Method**

- ForEach is used for iterating over every single element of array and printing them.

```javascript
var fruits = ["mango", "orange", "apple"];

fruits.forEach((fruit) => {
  console.log(fruits);
});
```

2.) **MAP Method**

- Map is used for transforming array but have to return something.

- It returns another array it doesn't change the original array.

```javascript
var sports = ["tennis", "football", "hockey"];

var another_arr = sports.map((sport) => {
  return sport + "Great";
});
```

3.) **FILTER Method**

- When we want to remove or filter some elements from the array we can use filter.

```javascript
var items = [10, "", 20, 30, null];

var filter_arr = items.filter((item) => {
  return !!item;
});
// All truthy values will get printed and falsy values will not get printed.
```
