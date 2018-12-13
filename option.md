# Option

## Options with defaults

```js
let options = {
  option1: 'MyOption'
};

let defaults = {
  option1: 'Hello',
  option2: 'World'
};

let o = Object.assign({}, defaults, options);
console.log(o.option1);
```

### After DOM has loaded

```js
document.addEventListener("DOMContentLoaded", function(e) {
  // Do something
});
```