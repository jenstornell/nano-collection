# String

## Replace line breaks with <br>

```js
let str = str.replace(/\n|\r\n|\r/g, '<br>');
```

## Remove extension from filename

https://stackoverflow.com/questions/1818310/regular-expression-to-remove-a-files-extension

```js
var input = 'myfile.png';
var output = input.substr(0, input.lastIndexOf('.')) || input;
```

## Get extension from filename

https://stackoverflow.com/questions/190852/how-can-i-get-file-extensions-with-javascript

```js
return filename.split('.').pop();
```

## Replace bracket tags

https://stackoverflow.com/questions/43931283/javascript-string-replace-short-tags-with-brackets

```js
var string = '<div id="test">A little [prefix] test</div>';
var replace = string.replace(/\[prefix\]/g, "replaced");
console.log(replace);
```