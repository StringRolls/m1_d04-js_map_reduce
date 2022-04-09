![logo_ironhack_blue 7](https://user-images.githubusercontent.com/23629340/40541063-a07a0a8a-601a-11e8-91b5-2f13e4e6b441.png)
# Module 1 - Day 4
# JS Advanced Array methods map(), reduce()


## Contents

> JS | Array advanced methods: `.map()`, `.reduce()`.
> JS | Reference VS value / Shadow copy VS deep copy


## Advanced Array methods

The `.map()` and `.reduce()` methods are methods of the Array object that do not mutate the original array.

- The `.map()` method:
  - Receives a function as an argument.
  - Returns a manipulated array of the same length as the original.
  - Transfers to each position of the resulting array the return of the argument function.
    ````javascript
    const values = [2, 4, 6] const doubledValues = [2, 4, 6].
    const doubledValues = values.map(elm => elm * 2) // [4, 8, 12].
    ````
- The `.reduce()` method: 
  - Receives as an argument a function with two default parameters: accumulator and iterated value.
  - Can receive a second argument as the initial value for the accumulator.
  - Takes as the value of the accumulator for the second and successive iterations the value returned from the previous iteration.
    ````javascript
    const values = [2, 4, 6] const sum = values.
    const sum = values.reduce((acc, elm) => acc + elm) // 12 
    ````
## Truthies VS falsies
The _falsie_ values (`null, undefined, false, NaN, 0, ''`) are rejected by default in conditional structures. Every other value (_truthy_) is accepted by default.

## Deep copy
It is possible to make a _deep_ copy of both an object/array and all objects/arrays inside it through the `JSON.parse(JSON.stringify(myArray))` technique (more info: [parse](1), [stringify](2)).

[1]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/JSON/parse
[2]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/JSON/stringify
