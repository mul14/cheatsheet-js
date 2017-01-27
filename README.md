# JavaScript Cheat Sheet

**Form**
* [Form Data](#formdata)

**Object**
* [Merge](#merge)

**Array**
* [Filter](#filter)
* [Find](#find)

**Iteration**
* [Iterate over object](#iterate-over-object)

**Data type**
* [Check if variable is an object](#check-if-variable-is-an-object)

## Form

### FormData

```js
const form = new FormData

form.append('name', 'Mulia')
form.append('name', 'Arifandi')
form.append('name', 'Nasution')

form.get('name') // Mulia
form.getAll('name') // ['Mulia', 'Arifandi', 'Nasution']
```

## Object

### Merge

```js
const first = { a: 1, b: 1 }
const second = { a: 2, c: 3 }
let result = {}

Object.assign({}, first, second) // { a: 2, b: 1, c: 3 }

Object.assign(result, first, second) // 'result' will be: { a: 2, b: 1, c: 3 }
```

## Array

### Filter

```js
const users = [
  { name: 'Mulia', age: 12 },
  { name: 'Arifandi', age: 26 },
  { name: 'Nasution', age: 32 },
]

users.filter(user => user.age > 17) 

// [{ name: 'Arifandi', age: 26 }, { name: 'Nasution', age: 32 }]
```

### Find

```js
const users = [
  { name: 'Mulia', age: 12 },
  { name: 'Arifandi', age: 26 },
  { name: 'Nasution', age: 32 },
]

users.find(user => user.age === 26) 

// { name: 'Arifandi', age: 26 }
```

## Iteration

### Iterate over object

```js
const item = {
  name: 'Susu',
  price: 100,
}

for (let i in item) {
  i // name, price
  item[i] // 'Susu', 100
}
```

## Data type

### Check if variable is an object

```js
const a = {}
a === Object(a) // true
```

Alternative

```js
const a = {}
a !== null && typeof a === 'object' // true
```
