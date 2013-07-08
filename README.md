math-helpers
===
Tiny statistics helper lib for node and the browser. Robust and fast.

## Installation

```
npm install math-helpers
```
(or just download math-helpers.js if you want to use it in the browser)


## Usage

Node (or with browserify)
```javascript
var math = require('math-helpers')(/* options */)

var avg = math.avg([1, 2, 3])
// TODO: document the other methods
```

Browser:

AMD (with a script load like require.js)
```javascript
define(['path/to/math-helpers'], function (mh) {
  var math = mh(/* options */)

  // use it...
})
```

Old and busted script tag (seriously, you shouldn't to that anymore :-P)
```html
<script src="fancy://cdn.com/math-helpers.js"></script>
<script>
  var math = window.MathHelpers(/* options */)
</script>
```

### Options

You can pass some options to the module.

```javascript
{
  precision: 3 // results will be rounded to this number of decimals
}
```