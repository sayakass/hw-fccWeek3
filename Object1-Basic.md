# Object (Basic : 13 ข้อ)

# Prerequisite

- array
- function (basic : parameter and return)

# Content

- Build JavaScript Objects
- Accessing Object Properties with Dot Notation
- Accessing Object Properties with Bracket Notation
- Accessing Object Properties with Variables
- Updating Object Properties
- Add New Properties to a JavaScript Object
- Delete Properties from a JavaScript Object
- Using Objects for Lookups
- Testing Objects for Properties
- Manipulating Complex Objects
- Accessing Nested Objects
- Accessing Nested Arrays
- Record Collection

# Basic

[1.Build JavaScript Objects](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/build-javascript-objects)

```js
const myDog = {
  // Only change code below this line
  name: 'krathin',
  legs: 4,
  tails: 1,
  friends: ['set', 'money'],

  // Only change code above this line
};
```

# Access Property and Value

[2.Accessing Object Properties with Dot Notation](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/accessing-object-properties-with-dot-notation)

```js
// Setup
const testObj = {
  hat: 'ballcap',
  shirt: 'jersey',
  shoes: 'cleats',
};

// Only change code below this line
const hatValue = testObj.hat; // Change this line
const shirtValue = testObj.shirt; // Change this line
```

[3.Accessing Object Properties with Bracket Notation](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/accessing-object-properties-with-bracket-notation)

```js
// Setup
const testObj = {
  'an entree': 'hamburger',
  'my side': 'veggies',
  'the drink': 'water',
};

// Only change code below this line
const entreeValue = testObj['an entree']; // Change this line
const drinkValue = testObj['the drink']; // Change this line
```

[4.Accessing Object Properties with Variables](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/accessing-object-properties-with-variables)

```js
// Setup
const testObj = {
  12: 'Namath',
  16: 'Montana',
  19: 'Unitas',
};

// Only change code below this line
const playerNumber = 16; // Change this line
const player = testObj[playerNumber]; // Change this line
```

# Update,Add,Delete Property and Value

[5.Updating Object Properties](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/updating-object-properties)

```js
// Setup
var myDog = {
  name: 'Coder',
  legs: 4,
  tails: 1,
  friends: ['freeCodeCamp Campers'],
};

// Only change code below this line
myDog['name'] = 'Happy Coder';
```

[6.Add New Properties to a JavaScript Object](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/updating-object-properties)

```js
const myDog = {
  name: 'Happy Coder',
  legs: 4,
  tails: 1,
  friends: ['freeCodeCamp Campers'],
};

myDog.bark = 'woof';
```

[7.Delete Properties from a JavaScript Object](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/delete-properties-from-a-javascript-object)

```js
// Setup
const myDog = {
  name: 'Happy Coder',
  legs: 4,
  tails: 1,
  friends: ['freeCodeCamp Campers'],
  bark: 'woof',
};

// Only change code below this line
delete myDog.tails;
```

# Intermediate

[8.Using Objects for Lookups](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/using-objects-for-lookups)\*ใช้เรื่องฟังก์ชันเล็กน้อย

```js
// Setup
function phoneticLookup(val) {
  let result = '';

  // Only change code below this line

  var lookup = {
    alpha: 'Adams',
    bravo: 'Boston',
    charlie: 'Chicago',
    delta: 'Denver',
    echo: 'Easy',
    foxtrot: 'Frank',
  };

  result = lookup[val];

  // Only change code above this line
  return result;
}

console.log(phoneticLookup('charlie'));
```

[9.Testing Objects for Properties](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/testing-objects-for-properties) \*ใช้เรื่องฟังก์ชันเล็กน้อย

```js
function checkObj(obj, checkProp) {
  if (obj.hasOwnProperty(checkProp)) {
    return obj[checkProp];
  } else {
    // Only change code below this line
    return 'Not Found';
  }
  // Only change code above this line
}
```

# Complex Object

[10.Manipulating Complex Objects](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/manipulating-complex-objects)

```js
const myMusic = [
  {
    artist: 'Billy Joel',
    title: 'Piano Man',
    release_year: 1973,
    formats: ['CD', '8T', 'LP'],
    gold: true,
  },
  {
    artist: 'Daft Punk',
    title: 'Homework',
    release_year: 1997,
    formats: ['CD', 'Cassette', 'LP'],
  },
];
```

[11.Accessing Nested Objects](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/accessing-nested-objects)

```js
const myStorage = {
  car: {
    inside: {
      'glove box': 'maps',
      'passenger seat': 'crumbs',
    },
    outside: {
      trunk: 'jack',
    },
  },
};

const gloveBoxContents = myStorage.car.inside['glove box'];
```

[12.Accessing Nested Arrays](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/accessing-nested-arrays)

```js
const myPlants = [
  {
    type: 'flowers',
    list: ['rose', 'tulip', 'dandelion'],
  },
  {
    type: 'trees',
    list: ['fir', 'pine', 'birch'],
  },
];

const secondTree = myPlants[1].list[1];
```

# Application

[13.Record Collection](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/record-collection)

```js
// Setup
var recordCollection = {
  2548: {
    albumTitle: 'Slippery When Wet',
    artist: 'Bon Jovi',
    tracks: ['Let It Rock', 'You Give Love a Bad Name'],
  },
  2468: {
    albumTitle: '1999',
    artist: 'Prince',
    tracks: ['1999', 'Little Red Corvette'],
  },
  1245: {
    artist: 'Robert Palmer',
    tracks: [],
  },
  5439: {
    albumTitle: 'ABBA Gold',
  },
};
// Only change code below this line
function updateRecords(records, id, prop, value) {
  if (prop !== 'tracks' && value !== '') {
    records[id][prop] = value;
  } else if (prop === 'tracks' && !records[id].hasOwnProperty('tracks')) {
    records[id][prop] = [value];
  } else if (prop === 'tracks' && value !== '') {
    records[id][prop].push(value);
  } else if (value === '') {
    delete records[id][prop];
  }
  return records;
}
updateRecords(recordCollection, 5439, 'artist', 'ABBA');
```
