# STRINGS

---

## 1. String Creation

---

- Strings are present in text and are wrapped in "DOUBLE QUOTES"

```javascript
var a = "My name is Manish";
console.log(a);

output -
My name is Manish
```

## 2. Built In Methods Of Strings

---

| Method       | How to write                      | Description                       |
| ------------ | --------------------------------- | --------------------------------- |
| .toLowercase | name.toLowercase()                | Coverts the string to lowercase   |
| .toUppercase | name.toUppercase()                | Coverts the string to upper case  |
| .split       | name.split("js")                  | Splits the string                 |
| .replace     | name.replace("oldText","newText") | Replace string with another value |
| .trim        | name.trim()                       | Removes the spaces which is extra |

## 3. String Literals

---

- String literals are used with the help of "${variableName}".

- We have to use backtick character (`).

Example:

```javascript
let first = "Manish";
let last = "Football";

let new = `${first} like to play ${last}`

output - Manish likes to play Footbal
```
