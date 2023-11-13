# Title: Callbacks in JavaScript

## 1. Introduction

In JavaScript, a callback is a function passed as an argument to another function, to be executed later. This mechanism is fundamental to handling asynchronous operations and promoting modular code.

## 2. Definition and Purpose

### 2.1 What is a Callback?

A callback is a function provided to another function, which is then invoked after a particular operation or event. This enables non-blocking execution, essential for handling asynchronous tasks.

### 2.2 Purpose of Callbacks

Callbacks facilitate the execution of functions in response to events, making them pivotal in scenarios like handling user input, making API requests, or reading files asynchronously.

## 3. Practical Applications

### 3.1 Event Handling

```javascript
document.getElementById('myButton').addEventListener('click', function() {
  console.log('Button clicked!')
})
```

### 3.2 Asynchronous Operations

```javascript
fetch('https://api.example.com/data')
  .then(response => response.json())
  .then(data => {
    process(data, function() {
      console.log('Processing complete!')
    })
  })
```

### 3.3 Timer Functions

```javascript
setTimeout(function() {
  console.log('Delayed message')
}, 2000)
```

## 4. Error Handling with Callbacks

### 4.1 Handling Errors

Callbacks can be used to handle errors in asynchronous operations, enhancing the robustness of the code.

```javascript
function fetchData(url, successCallback, errorCallback) {
  fetch(url)
    .then(response => response.json())
    .then(data => successCallback(data))
    .catch(error => errorCallback(error))
}

fetchData(
  'https://api.example.com/data',
  function(data) {
    console.log('Data received:', data)
  },
  function(error) {
    console.error('Error fetching data:', error)
  }
)
```
