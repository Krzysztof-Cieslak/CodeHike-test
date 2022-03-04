# Hello, world!

## Basic sample

<CH.Code>

```js app.js focus=2:4
function lorem(ipsum, dolor = 1) {
  const sit = ipsum == null ? 0 : ipsum.sit;
  dolor = sit - amet(dolor);
  return sit ? consectetur(ipsum) : [];
}
```

```python hello.py
print("Hello, world!")
```

---

```css styles.css
.lorem {
  color: #fff;
  padding: 10px;
  background: #000;
}
```

</CH.Code>


## Comment annotations

You can use comments inside the code to make the focus relative.

```js
function lorem(ipsum, dolor = 1) {
  const sit = ipsum == null && 0;
  dolor = sit - amet(dolor);
  // focus
  return sit ? consectetur(ipsum) : [];
}

// focus(1:4)
function adipiscing(...elit) {
  console.log(elit);
  return elit.map((ipsum) => ipsum.sit);
}

// focus[13:17]
console.log("hey");
```

Same with other annotations like `bg` and `box`.

```js
// bg(1:2)
function foo() {
  console.log("hover me");
  // box[3:10]
  return 8;
}
```

And now we introduce two more annotations: `link` and `label`

```js focus=4,8
function lorem(ipsum, dolor = 1) {
  const sit = ipsum == null && 0;
  dolor = sit - amet(dolor);
  // link[16:26] https://github.com/code-hike/codehike
  return sit ? consectetur(ipsum) : [];
}

function adipiscing(...elit) {
  // label something something
  console.log("hover me");
  return elit.map((ipsum) => ipsum.sit);
}
```

## Spotlight

This is how to use the `<CH.Spotlight>` component. Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam, quia! Quidem, quisquam.

<CH.Spotlight>

```js app.js
function lorem(ipsum, dolor = 1) {
  const sit = ipsum == null && 0;
  dolor = sit - amet(dolor);
  return sit ? consectetur(ipsum) : [];
}
```

---

Change focus

```js app.js focus=2:4

```

---

Or change the code

```js app.js focus=6:10
function lorem(ipsum, dolor = 1) {
  const sit = ipsum == null && 0;
  dolor = sit - amet(dolor);
  return sit ? consectetur(ipsum) : [];
}

function adipiscing(...elit) {
  console.log(elit);
  return elit.map((ipsum) => ipsum.sit);
}
```

---

Or change the file

<CH.Code>

```js app.js focus=1:4
function adipiscing(...elit) {
  console.log(elit);
  return elit.map((ipsum) => ipsum.sit);
}
```

---

```css styles.css
.lorem {
  color: #fff;
  padding: 10px;
  background: #000;
}
```

</CH.Code>

---

### By the way

- you can
- put any
- markdown
- here

👍

```js app.js

```

</CH.Spotlight>
