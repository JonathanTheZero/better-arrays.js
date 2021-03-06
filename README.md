# better-arrays.js
Better-arrays.js is a library to improve working with arrays in JavaScript and TypeScript.

## Set-Up:
Install the module with `npm i better-arrays.js`.
Use it in JavaScript with
```js
require("better-arrays.js"); //ES6 or
require("better-arrays.js/ES5/"); //ES5
```
The library is written in TypeScript and can be used with
```ts
import "better-arrays.js"; //or
import "better-arrays.js/ts/" //to directly include the TypeScript files
```

## Functions:

### Array.selectRandom(n?: number)
The Array.selectRandom method selects n random elements out of an array and returns them as a new array, the default is 1.

### Array.selectOneItem(minIndex?: number, maxIndex?: number)
This functions returns one random item out of the array as an object. The optional parameters `minIndex` defines a starting index for the method to search, while the optional parameter `maxIndex` defines an ending index.

### Array.deepcopy()
Returns a new array which is a deep copy of the old one.

### Array.shallowCopy()
Returns a new array which is a shallow copy of the old one.

### Array.toStringArray()
Returns a new array in which all elements have been parsed to strings.

### Array.toFloatArray(includeNaNs?: boolean)
Returns a new array in which all elements have been parsed to floats. The parameter `includeNaNs` specifies whether NaN values should be kept in the Array or not, default is false.

### Array.toIntArray(includeNaNs?: boolean)
Returns a new array in which all elements have been parsed to integers. The parameter `includeNaNs` specifies whether NaN values should be kept in the Array or not, default is false.

### Array.sortNumeric()
Sorts all values in the array numeric ascending.

### Array.delete(item: T)
Deletes every instance of the given item out of the array wihtout chaning the indices of the other items.

### Array.replace(oldItem: T, newItem: T)
Replaces all instances of `oldItem` with `newItem`.