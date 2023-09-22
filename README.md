# JavaScript Array Functions Practice

### you can use `Replit` an online IDE where you can run, share code 
### instructions: 
1. visit [Replit](https://replit.com/login?source=home&goto=%2F%7E&code=4131df8735dfb18d74bec4e3ec48d7e22d21b8d334b6f6056fb230b05f0de52a)
2. sign up with your email
3. Fork this [repl](https://replit.com/@adamMarey/Array-methods-practice-1?v=1)
4. have fun! 

Here's a sample piece of Star Wars data from the [Star Wars API](https://swapi.dev/).

## Sample Data
```javascript
const characters = [
    {
        name: 'Luke Skywalker',
        height: '172',
        mass: '77',
        eye_color: 'blue',
        gender: 'male',
    },
    {
        name: 'Darth Vader',
        height: '202',
        mass: '136',
        eye_color: 'yellow',
        gender: 'male',
    },
    {
        name: 'Leia Organa',
        height: '150',
        mass: '49',
        eye_color: 'brown',
        gender: 'female',
    },
    {
        name: 'Anakin Skywalker',
        height: '188',
        mass: '84',
        eye_color: 'blue',
        gender: 'male',
    },
];
```

## forEach  [mdn link](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/forEach)

1. Log each character's name to the console.
2. Log each character's height to the console.
3. Log a statement about each character (e.g., "Luke Skywalker is 172 cm tall and weighs 77 kg.").
4. Log each character's eye color.

## indexOf [mdn link](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/indexOf)

1. Find the index of the character with the name 'Darth Vader'.
2. Find the index of the first character with blue eyes.
3. Find the index of a character with a height of '150'.
4. Determine if there's a character named 'Obi-Wan Kenobi' (Hint: check if the result is -1).

## includes   [mdn link](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/includes)

1. Check if there's a character with the name 'Luke Skywalker'.
2. Check if there's a character with a mass of '85'.
3. Check if there's a character with the eye color 'green'.
4. Check if there's a character with the gender 'non-binary'.

## SORT   [mdn link](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/sort)

1. Sort by name in reverse order.
2. Sort by mass in descending order.
3. Sort by height in ascending order.
4. Sort by gender alphabetically.

## MAP  [mdn link](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/map)

1. Get an array of all names
2. Get an array of all heights
3. Get an array of objects with just name and height properties
4. Get an array of all first names

## REDUCE  [mdn link](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/reduce)

1. Get the total mass of all characters
2. Get the total height of all characters
3. Get the total number of characters in all the character names
4. Get the total number of characters by eye color (hint. a map of eye color to count)

## FILTER   [mdn link](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/filter)

1. Get characters with mass greater than 100
2. Get characters with height less than 200
3. Get all male characters
4. Get all female characters


