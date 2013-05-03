Hapt
====

Hapt is a javascript library for listening key bindings.

Example
-------

```javascript
// load hapt.js before executing following scripts.

hapt.listen(function(keys){
  switch (keys.join(' ')) {
    case 'E':
      // do something.
      return false; // prevent event propagation.
    case 'Shift Alt A':
      // do something.
      return false;
  }
  return true;
});
```