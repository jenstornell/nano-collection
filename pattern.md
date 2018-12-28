# Pattern

## Class (ES6)

```js
class Defaults {
  myExtended() {
    return 'Hello';
  }
}

class MyClass extends Defaults {
  constructor(options) {
    super();
  }

  myMethod(str) {
    return this.myExtended() + str;
  }
}

let MyInstance = new MyClass();
let value = MyInstance.myMethod(' world');
console.log(value);
```

## Module (ES5)

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