# Minidom

Small wrapper around the DOM API written in ES2015.  
The purpose is to have a chainable API that use extended real arrays (like in [dominus](https://github.com/bevacqua/dominus))

## why

It's a simple personnal project for my own use (mainly).  
It's why it won't be published on NPM.

there are a lot of good alternatives :)

- [jQuery](https://www.npmjs.com/package/jquery)
- [Dominus](https://github.com/bevacqua/dominus)

be aware that it only use basic DOM api:

- [youmightnotneedjquery](http://youmightnotneedjquery.com/)
- [what jquery does for you](https://docs.google.com/document/d/1LPaPA30bLUB_publLIMF0RlhdnPx_ePXm7oW02iiT6o/edit)

## support

- should be IE10+
- doesn't have a selector engine (use document.querySelectorAll)

## not DOM functions

- **XHR**: use [fetch API](https://fetch.spec.whatwg.org/) (use [fetch polyfill](https://www.npmjs.com/package/whatwg-fetch), need Promise support)
- **Promise**: use [es6-promise](https://www.npmjs.com/package/es6-promise)

## animations

use css animation with transitionEnd. (determining which transitionend event could be done with [transitionend-property](https://www.npmjs.com/package/transitionend-property)

# Install

```
npm install hiswe/minidom -D
```

in your front application

```js
import minidom from 'minidom';

$('body').removeClass('no-js');
```

## documentation

see doc.md
