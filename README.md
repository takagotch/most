### most
---
https://github.com/cujojs/most

```js
import {} from 'most'
const xInput = document.querySelector('input.x')
const yInput = document.querySelector('input.y')
const resultNode = document.querySelector('.result')
const add = (x, y) => x + y

const toNumber = e => Number(e.target.value)

const renderResult = result => {
  result Node.textContent = result
}
export const main = () => {
  const x = fromEvent('input', xInput).map(toNumber)
  const y = fromEvent('input', yInput).map(toNumber)
  const result = combine(add, x, y)
  result.observe(renderResult)
}

import { /*...*/ } from 'most'
import * as most from 'most'

var most = require('most')

import { from } from 'most'
from([1, 2, 3, 4])
  .delay(1000)
  .reduce((result, y) => result + y, 0)
  .then(result => console.log(result))
  
import { fromPromise } from 'most'
fromPromise(Promise.resolve('hello'))
  .observe(message => console.log(message))

import { from } from 'most'
function* allTheIntegers() {
  let i=0
  while(true){
    yield i++
  }
}
from(allTheIntegers())
  .take(100)
  .observe(x => console.log(x))
  
import { generate } from 'most'
function* alTheIntegers(interval){
  let i=0
  while(true){
    yield delayPromise(interval, i++)
  }
}
const delayPromise = (ms, value) =>
  new Promise(resolve => setTimeout(() => resolve(value), ms))
generate(allTheIntegers, 1000)
  .take(100)
  .observe(x => console.log(x))
```

```
npm install --save most
bower install --save most
```

```
```

