# How to use the `forEach` Method in JavaScript
![computer with code](https://images.unsplash.com/photo-1524666643752-b381eb00effb?q=80&w=2071&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D)
## Introduction

The `forEach()` method allows you to iterate over and perform 
operations on the elements of an array. It is a built-in JavaScript method.

## Syntax
```javascript
array.forEach(function(currentValue, index, array) {
  
  // code to perform on each array element

}, thisValue)
```

## Parameters

**function()**: Required. Can also replace with a callback function.

**currentValue**
Required: This is the value of the current element.

**index**: Optional The current element's index

**array**: Optional. The current element's array.

**thisValue**: Optional. Default undefined. Value to use when executing the callback function.

## Examples

### Call a function to print out the name of each car in the array cars.

```javascript
const cars = ["Chevy", "Ford", "Dodge"];

cars.forEach(function(car) {
  console.log(car);
});
```
### Call a function to find the total sum of an array of numbers.

```javascript
let sum = 0;
const numbers = [1, 2, 3];

numbers.forEach(sumArray);

//callback function
function sumArray(number) {
  sum += number;
}
```

## Considerations

1. The `forEach` method does not return an new array.

2. It does not work for object.

For more information, see the [MDN docs](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/forEach).