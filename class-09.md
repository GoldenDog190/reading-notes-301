# Online Readings

## [Functional Programming Concepts](https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa)

**Concepts of Functional Programming in Javascript**

* Functional Programming - a programming paradigm, which is a style of building the structure and elements of computer programs that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data.
* Pure functions - return the same result if given the same arguments, and it does not cause any observable side effects. 
  - Are stable, consistent, and predictable. Given the same parameters, pure functions will always return the same result.
  - Benefits: code will be easier to test, and don't need to mock anything, so can unit test pure functions with different contexts.
* Impure function - uses a global object that was not passed as a parameter to the function, its a function reads exernal files and file's contents can change, or relies on random number generator.
* Immutability - unchanging over time or unable to be changed. When data is immutable, its state cannot change after it’s created. Can't change, so you have to create a new object with a new value.
* Function composition or changing - to handle a mutation, which will result in a function being used as an input for the next function without modifying the original input string.
* Combine these 4 to slugify a string:
  - toLowerCase: converts the string to all lower case
  - trim: removes whitespace from both ends of a string
  - split and join: replaces all instances of match with replacement in a given string
* Referential transparency - a function that consistently yields the same result for the same input. pure functions + immutable data = referential transparency
* Functions as first-class entities - functions are treated as values and used as data. They can refer to it from constants and variables, pass it as a parameter to other functions, and return it as result from other functions.
* Higher-order functions - a function that either takes one or more functions as arguments, or returns a function as its result.
* Filter function - expects a true or false value to determine if the element should or should not be included in the result collection. 
* Imperative approach/way - create an empty array evenNumbers, iterate over the numbers array, and push the even numbers to the evenNumbers array.
*  Filter Array problem - problem idea is to filter a given array of integers and output only those values that are less than a specified value X.
* Declarative approach: have a list, have a function, and filter list based on function.
* Map method - transforms a collection by applying a function to all of its elements and building a new collection from the returned values.
* Math.abs function - used to transform the value into its absolute value, and do the in-place update.
* Reduce - is to receive a function and a collection, and return a value created by combining the items.

## [Refactoring Javascript for Readability](https://dev.to/healeycodes/refactoring-javascript-for-performance-and-readability-with-examples-1hec)

**Refactoring JavaScript for Performance and Readability**
* Refractoring - seperate some logic and reduce the number of lines of code.
* Strategies on making clean code:
  - Return earliy from functions
  - Cache variables so functions can be read like sentences
  - Check for Web APIs before implementing your own functionality
* Get your code right the first time because it can be hard to go back later to refactor it. 
* Hash Function - used to map a given key to a location in the hash table. 

* Scenario 1 Example:
  - // Unrefactored code

const URLstore = [];

function makeShort(URL) {
  const rndName = Math.random().toString(36).substring(2);
  URLstore.push({[rndName]: URL});
  return rndName;
}

function getLong(shortURL) {
  for (let i = 0; i < URLstore.length; i++) {
    if (URLstore[i].hasOwnProperty(shortURL) !== false) {
      return URLstore[i][shortURL];
    }
  }
}

- // Refactored code

const URLstore = new Map(); // Change this to a Map

function makeShort(URL) {
  const rndName = Math.random().toString(36).substring(2);
  // Place the short URL into the Map as the key with the long URL as the value
  URLstore.set(rndName, URL);
  return rndName;
}

function getLong(shortURL) {
  // Leave the function early to avoid an unnecessary else statement
  if (URLstore.has(shortURL) === false) {
    throw 'Not in URLstore!';
  }
  return URLstore.get(shortURL); // Get the long URL out of the Map
}


* Scenario 2 Example:
  - // Unrefactored code

const friendlyWords = require('friendly-words');

function randomPredicate() {
  const choice = Math.floor(Math.random() * friendlyWords.predicates.length);
  return friendlyWords.predicates[choice];
}

function randomObject() {
  const choice = Math.floor(Math.random() * friendlyWords.objects.length);
  return friendlyWords.objects[choice];
}

async function createUser(email) {
  const user = { email: email };
  user.url = randomPredicate() + randomObject() + randomObject();
  await db.insert(user, 'Users')
  sendWelcomeEmail(user);
}

- // Refactored code

const friendlyWords = require('friendly-words');

const generateURL = user => {
  const pick = arr => arr[Math.floor(Math.random() * arr.length)];
  user.url = `${pick(friendlyWords.predicates)}-${pick(friendlyWords.objects)}` +
    `-${pick(friendlyWords.objects)}`; // This line would've been too long for linters!
};

async function createUser(email) {
  const user = { email: email };
  // The URL-creation algorithm isn't important to this function so let's abstract it away
  generateURL(user);
  await db.insert(user, 'Users')
  sendWelcomeEmail(user);
}