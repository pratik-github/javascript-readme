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
