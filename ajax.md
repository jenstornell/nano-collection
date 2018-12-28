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
}).then((response) => {
  return response.text();
}).then((text) => {
  var array = JSON.parse(text);
  console.log(array);
});
```