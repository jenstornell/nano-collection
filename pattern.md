# Pattern

## A module pattern

A skeleton of a module pattern.

```js
var myModule = (function () {
  var fn = {};

  fn.init = function(options) {
    // Do something
  };

  return fn;
})();
```

**How to use it:**

```js
myModule.init();
```

or...

```js
myModule.init({
  option1: 'ChangeMe!'
});
```