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