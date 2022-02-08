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

- **Conversion** `console.log(+'23');` type coercion. | convert into number

### Parsing in function

`console.log(Number.parseInt('30px', 10));`
`console.log(Number.parseInt('e23', 10)); `

## Checking if value is number

`console.log(Number.isFinite(20));` `console.log(Number.isFinite('20'));`

## Create Date

```
console.log(new Date(account1.movementsDates[0]));
console.log(new Date(0));
console.log(new Data(3 * 24 * 60 * 60 * 1000));
// working with date
const future = new Date(2037, 10, 19, 15, 23);
console.log(future);
console.log(future.getFullYear()); | never use .getYear
console.log(future.getMonth());
console.log(future.getDate());
console.log(future.getDay());
console.log(future.getHours());
console.log(future.getMinutes());
console.log(future.getSeconds());
console.log(future.toISOString()); | international

console.log(future.getTime());

console.log(Date.now());

future.setFullYear(2040);
console.log(future);
```

### Internationalizing Dates(intl) `labelDate.textContent = new Intl.DateTimeFormat('en-US').format(now);`

[Intl](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Intl)

## setTimeout()
