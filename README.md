# JavaScript Cheat Sheet

**Form**
* [Form Data](#formdata)

**Array**
* [Filter](#filter)
* [Find](#find)

**Iteration**
* [Iterate over object](#iterate-over-object)

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
