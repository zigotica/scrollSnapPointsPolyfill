# scroll Snap Points Polyfill
===========================

Tiny Javascript Pollyfill to simulate CSS scroll Snap Points in non-supporting browsers. 


## Setup

1. Include the script at the end of your HTML, it will autorun when DOM is ready. 
2. Enjoy.

## Options

### Run after DOM injection
You can also run the script manually. Usefull when you dynamically inject nodes into your document. 

```
// your DOM injecton here
// then:
znapscroll.prepare();
```

### Destroy after DOM removal
Since you might want to remove elements from the DOM, we need to make sure memory is not leaked.


```
// your DOM removal here
// then:
znapscroll.destroy();
```

### Destroy limiting by context

`destroy` method accepts a context argument, to limit destruction to an HTML element:

```
// your DOM removal here
// then (limited to children of element with id=g1):
znapscroll.destroy( document.getElementById('g1') );
```