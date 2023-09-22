# forEach()
### Explanation:
The `forEach` function is used to loop over an array and perform some operation on each item.

```js

// 1. Log each character's name to the console.
characters.forEach(character => console.log(character.name));

// 2. Log each character's height to the console.
characters.forEach(character => console.log(character.height));

// 3. Log a statement about each character.
characters.forEach(character => console.log(`${character.name} is ${character.height} cm tall and weighs ${character.mass} kg.`));

// 4. Log each character's eye color.
characters.forEach(character => console.log(character.eye_color));
```

# indexOf()
### Explanation:
`indexOf` finds the index of the first item that satisfies a particular condition. It returns `-1` if no item is found.

```js
// Convert characters to an array of names for easier indexing
const names = characters.map(character => character.name);

// 1. Find the index of the character with the name 'Darth Vader'.
console.log(names.indexOf('Darth Vader'));

// 2. Find the index of the first character with blue eyes.
const blueEyedIndex = characters.findIndex(character => character.eye_color === 'blue');
console.log(blueEyedIndex);

// 3. Find the index of a character with a height of '150'.
const height150Index = characters.findIndex(character => character.height === '150');
console.log(height150Index);

// 4. Determine if there's a character named 'Obi-Wan Kenobi'.
console.log(names.indexOf('Obi-Wan Kenobi') !== -1);

```
# includes()
### Explanation:
`includes` checks if an array includes a certain value among its elements.

```js

// 1. Check if there's a character with the name 'Luke Skywalker'.
console.log(names.includes('Luke Skywalker'));

// 2. Check if there's a character with a mass of '85'.
console.log(characters.map(character => character.mass).includes('85'));

// 3. Check if there's a character with the eye color 'green'.
console.log(characters.map(character => character.eye_color).includes('green'));

// 4. Check if there's a character with the gender 'non-binary'.
console.log(characters.map(character => character.gender).includes('non-binary'));
```
# sort()
### Explanation:

`sort` arranges the elements of the array based on a comparator function.

```js
// 1. Sort by name in reverse order.
const sortedByName = [...characters].sort((a, b) => b.name.localeCompare(a.name));
console.log(sortedByName);

// 2. Sort by mass in descending order.
const sortedByMass = [...characters].sort((a, b) => b.mass - a.mass);
console.log(sortedByMass);

// 3. Sort by height in ascending order.
const sortedByHeight = [...characters].sort((a, b) => a.height - b.height);
console.log(sortedByHeight);

// 4. Sort by gender alphabetically.
const sortedByGender = [...characters].sort((a, b) => a.gender.localeCompare(b.gender));
console.log(sortedByGender);

```
# map()
### Explanation:
`map` creates a new array populated with the results of a function on every element in the calling array.

```js
// 1. Get an array of all names
const allNames = characters.map(character => character.name);
console.log(allNames);

// 2. Get an array of all heights
const allHeights = characters.map(character => character.height);
console.log(allHeights);

// 3. Get an array of objects with just name and height properties
const nameAndHeight = characters.map(({ name, height }) => ({ name, height }));
console.log(nameAndHeight);

// 4. Get an array of all first names
const firstNames = characters.map(character => character.name.split(' ')[0]);
console.log(firstNames);
```

# reduce()
### Explanation:

`reduce` applies a function against an accumulator and each value of the array to reduce it to a single value.

```js
// 1. Get the total mass of all characters
const totalMass = characters.reduce((acc, character) => acc + Number(character.mass), 0);
console.log(totalMass);

// 2. Get the total height of all characters
const totalHeight = characters.reduce((acc, character) => acc + Number(character.height), 0);
console.log(totalHeight);

// 3. Get the total number of characters in all the character names
const totalNameChars = characters.reduce((acc, character) => acc + character.name.length, 0);
console.log(totalNameChars);

// 4. Get the total number of characters by eye color
const eyeColorCount = characters.reduce((acc, character) => {
    acc[character.eye_color] = (acc[character.eye_color] || 0) + 1;
    return acc;
}, {});
console.log(eyeColorCount);
```

# filter()
### Explanation:
`filter` creates a new array with all elements that pass the test implemented by the provided function

```js
// 1. Get characters with mass greater than 100
const heavyCharacters = characters.filter(character => Number(character.mass) > 100);
console.log(heavyCharacters);

// 2. Get characters with height less than 200
const shortCharacters = characters.filter(character => Number(character.height) < 200);
console.log(shortCharacters);

// 3. Get all male characters
const maleCharacters = characters.filter(character => character.gender === 'male');
console.log(maleCharacters);

// 4. Get all female characters
const femaleCharacters = characters.filter(character => character.gender === 'female');
console.log(femaleCharacters);
```












