# JavaScript Cheatsheet

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

## DOM Manipulation

### Select Elements

```javascript
const elementById = document.getElementById('elementId');
const elementsByClass = document.getElementsByClassName('className');
const elementsByTag = document.getElementsByTagName('tagName');
const firstElementByQuery = document.querySelector('cssSelector');
const allElementsByQuery = document.querySelectorAll('cssSelector');
```

### Manipulate Elements

```javascript
element.textContent = 'New Text';
element.innerHTML = '<b>New HTML</b>';
element.style.property = 'value';
element.classList.add('newClass');
element.classList.remove('oldClass');
element.classList.toggle('toggleClass');
element.setAttribute('attributeName', 'attributeValue');
element.removeAttribute('attributeName');
```

## Array Methods

```javascript
arr.forEach((element, index) => {
  // Code to execute for each element
});

const newArray = arr.map((element, index) => {
  // Return the new element
});

const filteredArray = arr.filter((element, index) => {
  // Return true if the element should be included
});

const foundElement = arr.find((element, index) => {
  // Return true if this is the element you want to find
});

const someTruthy = arr.some((element, index) => {
  // Return true if some elements meet the condition
});

const allTruthy = arr.every((element, index) => {
  // Return true if all elements meet the condition
});

const reducedValue = arr.reduce((accumulator, element, index) => {
  // Return the new accumulator value
}, initialValue);
```

## String Methods

```javascript
const stringLength = str.length;
const newString = str.replace('search', 'replacement');
const stringIndex = str.indexOf('search');
const stringLastIndex = str.lastIndexOf('search');
const substring = str.slice(startIndex, endIndex);
const splitArray = str.split('separator');
```

## Import Statements for Webpack

```javascript
import moduleName from 'module';
import { namedExport } from 'module';
import { namedExport as alias } from 'module';
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
