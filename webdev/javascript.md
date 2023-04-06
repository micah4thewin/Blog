# JavaScript

## DOMContentLoaded

```javascript
document.addEventListener('DOMContentLoaded', () => {
  // Your code here
});
```

## If Statements

```javascript
if (condition) {
  // Code to execute if the condition is true
} else {
  // Code to execute if the condition is false
}
```

## setTimeout

```javascript
setTimeout(() => {
  // Code to execute after the specified delay
}, delayInMilliseconds);
```

## Event Handling

```javascript
element.addEventListener('eventType', (event) => {
  // Code to execute when the event occurs
});
```
```javascript
element.removeEventListener('eventType', eventListenerFunction);
```


## DOM Manipulation

### Select Elements

```javascript
const elementById = document.getElementById('elementId');
```
```javascript
const elementsByClass = document.getElementsByClassName('className');
```
```javascript
const elementsByTag = document.getElementsByTagName('tagName');
```
```javascript
const firstElementByQuery = document.querySelector('cssSelector');
```
```javascript
const allElementsByQuery = document.querySelectorAll('cssSelector');
```

### Manipulate Elements

```javascript
element.textContent = 'New Text';
```
```javascript
element.innerHTML = '<b>New HTML</b>';
```
```javascript
element.style.property = 'value';
```
```javascript
element.classList.add('newClass');
```
```javascript
element.classList.remove('oldClass');
```
```javascript
element.classList.toggle('toggleClass');
```
```javascript
element.setAttribute('attributeName', 'attributeValue');
```
```javascript
element.removeAttribute('attributeName');
```

### Create and Add Elements

```javascript
const newElement = document.createElement('tagName');
```
```javascript
newElement.textContent = 'New Text';
```
```javascript
newElement.classList.add('newClass');
```
```javascript
parentElement.appendChild(newElement);
```

### Insert Elements

```javascript
parentElement.insertBefore(newElement, referenceElement);
```

### Remove Elements

```javascript
parentElement.removeChild(childElement);
```

### Replace Elements

```javascript
parentElement.replaceChild(newElement, oldElement);
```
## Array Methods

```javascript
arr.forEach((element, index) => {
  // Code to execute for each element
});
```
```javascript
const newArray = arr.map((element, index) => {
  // Return the new element
});
```
```javascript
const filteredArray = arr.filter((element, index) => {
  // Return true if the element should be included
});
```
```javascript
const foundElement = arr.find((element, index) => {
  // Return true if this is the element you want to find
});
```
```javascript
const someTruthy = arr.some((element, index) => {
  // Return true if some elements meet the condition
});
```
```javascript
const allTruthy = arr.every((element, index) => {
  // Return true if all elements meet the condition
});
```
```javascript
const reducedValue = arr.reduce((accumulator, element, index) => {
  // Return the new accumulator value
}, initialValue);
```

## String Methods

```javascript
const stringLength = str.length;
```
```javascript
const newString = str.replace('search', 'replacement');
```
```javascript
const stringIndex = str.indexOf('search');
```
```javascript
const stringLastIndex = str.lastIndexOf('search');
```
```javascript
const substring = str.slice(startIndex, endIndex);
```
```javascript
const splitArray = str.split('separator');
```

## Import Statements for Webpack

```javascript
import moduleName from 'module';
```
```javascript
import { namedExport } from 'module';
```
```javascript
import { namedExport as alias } from 'module';
```
```javascript
import * as moduleName from 'module';
```

## Loops

### For Loop

```javascript
for (let i = 0; i < arr.length; i++) {
  // Code to execute for each iteration
}
```

### For...of Loop

```javascript
for (const element of arr) {
  // Code to execute for each element
}
```

### For...in Loop

```javascript
for (const key in object) {
  // Code to execute for each key
}
```

## Async and Promises

### Promise

```javascript
const promise = new Promise((resolve, reject) => {
  // Do async operation, resolve(value) if successful, reject(error) if failed
});

promise.then((value) => {
  // Code to execute when promise is resolved
}).catch((error) => {
  // Code to execute when promise is rejected
}).finally(() => {
  // Code to execute after either resolve or reject
  }).finally(() => {
  // Code to execute after either resolve or reject
});
```

### Async/Await

```javascript
async function asyncFunction() {
  try {
    const result = await promise;
    // Code to execute when promise is resolved
  } catch (error) {
    // Code to execute when promise is rejected
  } finally {
    // Code to execute after either resolve or reject
  }
}
```

## Fetch API

```javascript
fetch('https://api.example.com/data')
  .then((response) => response.json())
  .then((data) => {
    // Code to execute with fetched data
  })
  .catch((error) => {
    // Code to execute if the fetch fails
  });
```

## FormData

```javascript
const formData = new FormData(formElement);
fetch('https://api.example.com/submit', {
  method: 'POST',
  body: formData,
});
```

## Web Storage (localStorage & sessionStorage)

### Set Item

```javascript
localStorage.setItem('key', 'value');
sessionStorage.setItem('key', 'value');
```

### Get Item

```javascript
const value = localStorage.getItem('key');
```
```javascript
const value = sessionStorage.getItem('key');
```

### Remove Item

```javascript
localStorage.removeItem('key');
```
```javascript
sessionStorage.removeItem('key');
```

### Clear Storage

```javascript
localStorage.clear();
```
```javascript
sessionStorage.clear();
```

## Class Example with Getters and Setters

```javascript
class MyClass {
  constructor(initialValue) {
    this._property = initialValue;
  }

  // Getter
  get property() {
    return this._property;
  }

  // Setter
  set property(newValue) {
    this._property = newValue;
  }

  // Method
  myMethod() {
    // Code to execute
  }
}

const myInstance = new MyClass('initialValue');
```

## Unique ID

```javascript
function generateUniqueId() {
  return Date.now().toString(36) + Math.random().toString(36).substr(2);
}

const uniqueId = generateUniqueId();
```

## Dates and Date Formatting

```javascript
const currentDate = new Date();
```
```javascript
const specificDate = new Date('2022-01-01T00:00:00');
```
```javascript
const year = currentDate.getFullYear();
```
```javascript
const month = currentDate.getMonth() + 1;
```
```javascript
const day = currentDate.getDate();
```
```javascript
const formattedDate = currentDate.toISOString();
```
```javascript
const formattedLocaleDate = currentDate.toLocaleDateString('en-US', {
  year: 'numeric',
  month: 'long',
  day: 'numeric',
});
```

## String Formatting

### Template Literals

```javascript
const name = 'John';
const age = 25;
const formattedString = `My name is ${name} and I am ${age} years old.`;
```

### String Concatenation

```javascript
const concatenatedString = 'My name is ' + name + ' and I am ' + age + ' years old.';
```

## Error Handling (try-catch-finally)

```javascript
try {
  // Code that may throw an error
} catch (error) {
  // Code to execute if an error occurs
} finally {
  // Code to execute after try and catch, regardless of whether an error occurred or not
}
```

## Regular Expressions

### Test for a Match

```javascript
const regex = /pattern/;
const str = 'string to test';
const hasMatch = regex.test(str);
```

### Find Matches and Capture Groups

```javascript
const matches = str.match(regex);
```

### Replace with Regular Expressions

```javascript
const replacedStr = str.replace(regex, 'replacement');
```

## JSON

### Parse JSON

```javascript
const jsonString = '{"key": "value"}';
const jsonObject = JSON.parse(jsonString);
```

### Stringify JSON

```javascript
const jsonObject = { key: 'value' };
const jsonString = JSON.stringify(jsonObject);
```

## Destructuring Assignment

### Arrays

```javascript
const [a, b] = [1, 2];
```

### Objects

```javascript
const { key1, key2 } = { key1: 'value1', key2: 'value2' };
```

## Spread and Rest Operators

### Spread Operator

```javascript
const newArray = [...oldArray, newItem];
const newObject = { ...oldObject, newKey: 'newValue' };
```

### Rest Operator

```javascript
function myFunction(...args) {
  // args is an array of arguments
}
```

## Arrow Functions

```javascript
const myFunction = (parameter) => {
  // Code to execute
};
```

## Modules

### Export

```javascript
export const myVariable = 'value';
export function myFunction() { /* Code to execute */ }
```

### Import

```javascript
import { myVariable, myFunction } from './myModule.js';
```

```javascript
const num = 4.9;
const roundedNum = ~~num; // 4
```

## Short-circuit Evaluation

```javascript
const defaultValue = 'Default';
const value = userInput || defaultValue;
```

## Exponentiation Operator (**)

```javascript
const square = 2 ** 2; // 4
const cube = 2 ** 3; // 8
```

## Quick Array Type Check

```javascript
const isArray = (arr) => arr.constructor === Array;
```

## Remove Array Duplicates

```javascript
const uniqueArray = [...new Set(array)];
```

## Shorthand Object Properties

```javascript
const a = 1;
const b = 2;
const obj = { a, b }; // { a: 1, b: 2 }
```

## Shorthand Functions

```javascript
const myFunc = (a, b) => a + b;
```

## Optional Chaining

```javascript
const value = obj?.nestedObj?.property;
```


## Double tilde

```javaScript
const num = 4.9;
const roundedNum = ~~num; // 4
```

## Nullish Coalescing Operator (??)'

```javascript
const result = value ?? defaultValue; // defaultValue if value is null or undefined
```

## Mouse Events

```
- click
- dblclick
- mousedown
- mouseup
- mousemove
- mouseover
- mouseout
- contextmenu
```

## Keyboard Events

```
- keydown
- keyup
- keypress
```

## Form Events

```
- submit
- change
- focus
- blur
```

## Window Events

```
- load
- unload
- beforeunload
- error
- resize
- scroll
```

## Drag & Drop Events

```
- drag
- dragstart
- dragend
- dragenter
- dragover
- dragleave
- drop
```

## Touch Events

```
- touchstart
- touchend
- touchmove
- touchcancel
```

## Pointer Events

```
- pointerover
- pointerenter
- pointerdown
- pointermove
- pointerup
- pointercancel
- pointerout
- pointerleave
- gotpointercapture
- lostpointercapture
```
