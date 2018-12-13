# Ajax

## Send POST with Ajax - Get JSON back

```js
var data = {};
data[id] = 1;

json = JSON.stringify(data);

fetch('api/?page=api&action=edit', {
  method: 'POST',
  body: json,
  headers: {
    "Content-Type": "Content-Type: application/json"
},
}).then(function(response) {
  return response.text();
}).then(function(text) {
  var array = JSON.parse(text);
  console.log(array);
});
```

### Check if JSON is valid

```js
function isJson(str) {
  try {
    JSON.parse(str);
  } catch (e) {
    return false;
  }
  return true;
}
```