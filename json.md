# Json

## Json encode and decode

```js
var data = {};
data[id] = 1;

let json = JSON.stringify(data);
let array = JSON.parse(json);
```

## Is Json

```js
function isJson(str) {
  try {
    JSON.parse(str);
  } catch (e) {
      return false;
  }
  return true;
  }
}

console.log(isJson('{test}'));
```