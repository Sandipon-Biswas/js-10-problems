
# Javascript 10 problems for beginners 






## Problem 1

Write a function that takes in a string and returns the string with all vowels removed.

```bash
function removeVowels(str) {
  // Initialize a variable to store the result
  let result = "";

  // Use a for loop to iterate over the characters in the string
  for (const ch of str) {
    // If the character is not a vowel, add it to the result string
    if (ch !== "a" && ch !== "e" && ch !== "i" && ch !== "o" && ch !== "u") {
      result += ch;
    }
  }

  // Return the result string
  return result;
}

// Test the function
console.log(removeVowels("hello")); // "hll"
console.log(removeVowels("aeiou")); // ""
console.log(removeVowels("abcde")); // "bcde"
```


## Problem 2
Write a function that takes in an array of strings and returns an array of the strings sorted alphabetically.


```bash
function sortStrings(strings) {
  // Use the sort method to sort the strings alphabetically
  return strings.sort();
}

// Test the function
console.log(sortStrings(["c", "b", "a"])); // ["a", "b", "c"]
console.log(sortStrings(["apple", "banana", "cherry"])); // ["apple", "banana", "cherry"]
console.log(sortStrings(["abc", "def", "ghi"])); // ["abc", "def", "ghi"]
```
## Problem 3
Write a function that takes in an array of numbers and returns the smallest number in the array.


```bash
function findSmallest(numbers) {
  // Use the Math.min function to find the smallest number in the array
  return Math.min(...numbers);
}

// Test the function
console.log(findSmallest([1, 2, 3])); // 1
console.log(findSmallest([4, 5, 6])); // 4
console.log(findSmallest([7, 8, 9])); // 7
```
## Problem 4
Write a function that takes in an array of numbers and returns the largest number in the array.


```bash
function findLargest(numbers) {
  // Use the Math.max function to find the largest number in the array
  return Math.max(...numbers);
}

// Test the function
console.log(findLargest([1, 2, 3])); // 3
console.log(findLargest([4, 5, 6])); // 6
console.log(findLargest([7, 8, 9])); // 9
```
## Problem 5

Write a function that takes in an array of numbers and returns the average of all the numbers in the array.

```bash
function findAverage(numbers) {
  // Initialize a variable to store the sum of the numbers
  let sum = 0;

  // Use a for loop to iterate over the numbers and add them to the sum
  for (const number of numbers) {
    sum += number;
  }

  // Return the average by dividing the sum by the number of numbers
  return sum / numbers.length;
}

// Test the function
console.log(findAverage([1, 2, 3])); // 2
console.log(findAverage([4, 5, 6])); // 5
console.log(findAverage([7, 8, 9])); // 8
```
## Problem 6

Write a function that takes in a string and returns the string with all characters in reverse order.

```bash
function reverseString(str) {
  // Use the split, reverse, and join methods to reverse the string
  return str.split("").reverse().join("");
}

// Test the function
console.log(reverseString("hello")); // "olleh"
console.log(reverseString("aeiou")); // "uoiea"
console.log(reverseString("abcde")); // "edcba"
```
## Problem 7
Write a function that takes in a string and returns the number of vowels in the string.


```bash
function countVowels(str) {
  // Initialize a variable to store the count of vowels
  let count = 0;

  // Use a for loop to iterate over the characters in the string
  for (const ch of str) {
    // If the character is a vowel, increment the count
    if (ch === "a" || ch === "e" || ch === "i" || ch === "o" || ch === "u") {
      count++;
    }
  }

  // Return the count
  return count;
}

// Test the function
console.log(countVowels("hello")); // 2
console.log(countVowels("aeiou")); // 5
console.log(countVowels("abcde")); // 2
```
## Problem 8

Write a function that takes in an array of numbers and returns an array of the numbers squared.

```bash
function squareNumbers(numbers) {
  // Initialize an empty array to store the squared numbers
  let squared = [];

  // Use a for loop to iterate over the numbers
  for (const number of numbers) {
    // Add the square of the number to the squared array
    squared.push(number * number);
  }

  // Return the squared array
  return squared;
}

// Test the function
console.log(squareNumbers([1, 2, 3])); // [1, 4, 9]
console.log(squareNumbers([4, 5, 6])); // [16, 25, 36]
console.log(squareNumbers([7, 8, 9])); // [49, 64, 81]
```
## Problem 9
Write a function that takes in an array of strings and returns an array of the strings with all characters in uppercase.


```bash
function toUppercase(strings) {
  // Initialize an empty array to store the uppercase strings
  let uppercase = [];

  // Use a for loop to iterate over the strings
  for (const str of strings) {
    // Add the uppercase version of the string to the uppercase array
    uppercase.push(str.toUpperCase());
  }

  // Return the uppercase array
  return uppercase;
}

// Test the function
console.log(toUppercase(["a", "b", "c"])); // ["A", "B", "C"]
console.log(toUppercase(["apple", "banana", "cherry"])); // ["APPLE", "BANANA", "CHERRY"]
console.log(toUppercase(["abc", "def", "ghi"])); // ["ABC", "DEF", "GHI"]
```
## Problem 10

Write a function that takes in an array of numbers and returns true if all the numbers in the array are positive, and false otherwise.

```bash
function arePositive(numbers) {
  // Use the every method to check if all numbers are positive
  return numbers.every(number => number > 0);
}

// Test the function
console.log(arePositive([1, 2, 3])); // true
console.log(arePositive([4, 5, 6])); // true
console.log(arePositive([7, 8, 9])); // true
console.log(arePositive([1, -2, 3])); // false
console.log(arePositive([4, 5, -6])); // false
console.log(arePositive([-7, 8, 9])); // false
```
