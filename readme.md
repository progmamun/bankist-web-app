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
