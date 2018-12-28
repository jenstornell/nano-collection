# Form

## Get values from a select multiple form element

https://stackoverflow.com/questions/9602449/a-javascript-design-pattern-for-options-with-default-values

```js
function getSelectedValues(sel) {
  var opts = [], opt;
  
  for (var i=0, len=sel.options.length; i<len; i++) {
      opt = sel.options[i];
      
      if ( opt.selected ) {
          opts.push(opt);
      }
  }
  
  return opts;
}
```

## Get select option label

```js
let element = document.querySelector('select');
let label = element.options[element.selectedIndex].text;
```

## Get options

```js
function options(el) {
  let options = {};

  Array.from(el.options).forEach((option) => {
      if(option.selected) {
      options[option.value] = option.textContent;
      }
  });

  return options;
};

var element = document.querySelector('select');
var my_options = options(element);
console.log(my_options);
```