# JavaScript General Notes


### Table of Contents

| No. | Questions |
|---- | ---------
|1  | [What are the difference between Object vs Map?](#01) |

1. ### What are the difference between Object vs Map?
 - Declaration- object can be declared in many ways whereas for map we use new Map(..)
 - The `key / value` in Map can be of any datatype whereas for object key can be – integer, string or symbol
 - In Map – order of elements is preserved
 - Map is an instance of object
 - Access element- `map.get(index)`
 - Add/update element- `map.set(index, value)`
 - Removing/deleting an element
   - object: no built in method can be done using delete obj.key / obj.key = undefined
   - `map.delete(index) / map.clear()` // delte all
 - Getting size / length
   - object: no built in method .. Object.keys (..).length
   - `map.size`
 - map is iterable whereas object doesn’t
 - JSON has direct support for Object, but not with Map (yet)
 - map- perform better in storing large set of data and which need frequest add/delete operations

 For additional information refer: https://medium.com/front-end-weekly/es6-map-vs-object-what-and-when-b80621932373 

2. ### IIFE
 - Is a JavaScript function that runs as soon as it is defined.
 - Lexical scope ... () ... This prevents accessing variables within the IIFE idiom as well as polluting the global scope.
 - That’s a function that died immediately after it came to life.
 - prefixing “!” in-front of the function keyword on line 1. This basically enforces JavaScript to treat whatever that’s coming after “!” as an expression
- Advantages/Benefits
   1. local scoping (prevents accessing variables within + polluting global scope)
   2. reduces scope lookup (performance benefit)
   3. we can pass global objects and reference within IIFE via local scope
   4. Helps minification optimisation => passing global objects as local values (paramters), allows minifier to reduce it to one letter... i.e. minify .. eg: window to w, jQuery to $.

Additional references:
 - http://gregfranko.com/blog/i-love-my-iife/ 
 - https://medium.com/@vvkchandra/essential-javascript-mastering-immediately-invoked-function-expressions-67791338ddc6 

