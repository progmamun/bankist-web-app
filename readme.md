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

## **Map Method:**

- map returns a **new array** containing the result of applying an operation on all original array elements.

## **Filter Method:**

- filter returns a **new array** containing the array elements that passed a specified **test condition**.

## **Reduce Method:**

- reduce boils ("reduces") all array elements down to one single value (e.g. adding all elements together)
- first parameter call **accumulator** . | like _SNOWBALL_| 2nd parameter **current value** .

## Flat | flatMap

## Sorting

`return < 0, A, B, C (keep order)| return > 0, C, B, A (switch order)`

- **String and number together it's not work**

```
// Ascending
movements.sort((a, b) => {
  if (a > b) return 1;
  if (a < b) return -1;
});
// or
movements.sort((a, b) => a - b);

// Descending
movements.sort((a, b) => {
  if (a > b) return -1;
  if (a < b) return 1;
});
// or
movements.sort((a, b) => b - a);
```

## Empty arrays | fill method | Array.from method

`const y = Array.from({ length: 7 }, () => 1);`
`const z = Array.from({ length: 100 }, (_, i) => i++);`
