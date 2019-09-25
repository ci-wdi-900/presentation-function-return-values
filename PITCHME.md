---
marp: true
title: Web Development Orientation
theme: uncover
---

<!-- backgroundColor: #393D3F -->
<!-- color: #D7FFF1-->
<style>
  code, pre {
    background-color: #393D3F;
    color: #D7FFF1;
  }
</style>

### The Final Function Technique

![w:800](https://media.moddb.com/images/downloads/1/60/59795/return_6.jpg)

---

### What's `return` FOR?

Parameters let us give input to our functions; `return` gives us output!

![w:500](http://pluspng.com/img-png/input-output-machine-png-asynchronous-1600.png)

---

### How's It Work?

```javascript
function exclaim(greeting) {
  const yelled = greeting + '!';

  return yelled;
}
```

Whatever is immediately after `return` becomes the output of our function!

---

### Now We Can USE That Output

```javascript
function exclaim(greeting) {
  const yelled = greeting + '!';

  return yelled;
}

const yelledGreeting = exclaim('Hi');
console.log(yelledGreeting); // -> 'Hi!'
```

---

### Our Functions Evaluate Now

The "return value" is what we decide the function evaluates to.

```javascript
const yelledGreeting = exclaim('Hi');
```

`exclaim('Hi')` evaluates to `'Hi!'`, so we can take that value and put it in a variable!

---

### Now Instead Of This:

```javascript
let x = 3;

function add5() {
  x = x + 5;
}
```

---

### We Can Do This:

```javascript
const x = 3;
const y = 15;

function add5(num) {
  return num + 5;
}

const bumpedX = add5(x);
const bumpedY = add5(y);
```

---

### All Functions Return SOMETHING

But if you don't explicitly return, JavaScript returns `undefined` for you.

```javascript
function whoopsForgotToReturn(x, y) {
  const sum = x + y;
}

const oopsie = whoopsForgotToReturn(5, 15);

console.log(oopsie); // -> undefined
```

---

# Now You Have... `return`!!!

![w:300](https://thumbs.gfycat.com/FaithfulLawfulKusimanse-max-1mb.gif)