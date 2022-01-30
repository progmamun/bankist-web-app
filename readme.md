# simple but advanced array-methods **ES6/ES7 and so on**

- **Splice method:** mute the original array
- **Slice method:** doesn't mute original array create new one

---

- **Reverse method:** mute original array
- **Concat method:** doesn't mute original array
- **Join method:**

---

- **forEach:** higher order function

```
const movements = [200, 450, -400, 3000, -650, -130, 70, 1300];
movements.forEach(function (movement) {
  if (movement > 0) {
    console.log(`You deposited ${movement}`);
  } else {
    console.log(`You withdrew ${Math.abs(movement)}`);
  }
});

```

movements.forEach(function (movement, index, array) {}

- first parameter the current element , second parameter always the current index of array, third one always the entire array

---

- [insertAdjacentHTML](https://developer.mozilla.org/en-US/docs/Web/API/Element/insertAdjacentHTML)
  `element.insertAdjacentHTML(position, text); `
