# Static methods

### minidom(selector:string | minidom | single DOMel, [context])

return a minidom collection.  
Context is the same as in jQuery.  
minidom(string) won't parse SVG :S

### hasSupport()

```js
import {default as minidom, hasSupport} from 'minidom';
```

return a boolean.
Check the presence of `querySelector` and `addEventListener`.

`warning`: this doesn't check [classList](http://caniuse.com/#feat=classlist) for example

### Instance Methods

# ATTRIBUTES / CSS

## Attributes

### a.addClass(value) 

white space separated list of classes.  
return minidom

### a.attr(name, [value]) 

- getter: return attribute value
- setter: return minidom

### a.hasClass(name)

return boolean

### a.removeClass(value) 

white space separated list of classes.  
return minidom

## CSS

### a.css(property, [value])

- getter: return CSS value
- setter: return minidom

# MANIPULATION

## DOM Insertion, Inside

### a.append(childrens:string | childrens:minidom | childrens:DOMel)

return minidom

### a.html(content:string)

return minidom

### a.prepend(content:string | content:minidom } content:DOMel)

return minidom

## DOM Removal

### a.remove()

return empty minidom

# TRAVERSING

## Filtering

### a.eq(index:number)

return a minidom at the index.  
(a[index] will ge the raw DOMel)

## Miscellaneous Traversing

### a.add(selector:string | minidom | single DOMel)

a return a minidom with those elements added.  
merge minidom set can also be acheived by a.push(...b);

## Tree traversal

### a.find(selector:string)

return a new minidom

### a.parent(selector:string)

return a new minidom

# EVENTS

## Event Handler Attachment

### a.on(eventName:string, callback:function)

return a new minidom

# core

## DOM Element Methods

### a.index(el:minidom | el:DOMel)

return index in the minidom list  
finding a DOMel can also be achieved by a.indexOf(el:DOMel)
