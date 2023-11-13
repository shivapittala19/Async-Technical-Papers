# Title: Code Control

## 1. **Conditionals (if-else statements):**

```javascript
let x = 10;

if (x > 0) {
  console.log('x is positive');
} else if (x === 0) {
  console.log('x is zero');
} else {
  console.log('x is negative');
}
```

## 2. **Switch Statement:**

```javascript
let day = 'Monday';

switch (day) {
  case 'Monday':
    console.log('It\'s the start of the week');
    break;
  case 'Friday':
    console.log('Weekend is near');
    break;
  default:
    console.log('It\'s a regular day');
}
```

## 3. **Loops (for, while, do-while):**

### 3.1 For Loop:

```javascript
for (let i = 0; i < 5; i++) {
  console.log(i);
}
```

### 3.2 While Loop:

```javascript
let i = 0;

while (i < 5) {
  console.log(i);
  i++;
}
```

### 3.3 Do-While Loop:

```javascript
let i = 0;

do {
  console.log(i);
  i++;
} while (i < 5);
```

## 4. **Break and Continue Statements:**

### 4.1 Break:

```javascript
for (let i = 0; i < 10; i++) {
  if (i === 5) {
    break;
  }
  console.log(i);
}
```

### 4.2 Continue:

```javascript
for (let i = 0; i < 10; i++) {
  if (i === 5) {
    continue;
  }
  console.log(i);
}
```

## 5. **Try-Catch Statement (Error Handling):**

```javascript
try {
  // code that might throw an error
  throw new Error('This is an error');
} catch (error) {
  console.error(error.message);
} finally {
  console.log('This will always execute');
}
```
