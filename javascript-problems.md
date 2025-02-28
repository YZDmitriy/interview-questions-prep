# Questions
## Array
- [Write a function to remove duplicates in an array, sort it in the descending order.](#QA1)
- [How to empty an array.](#QA2)
- [Remove duplicate values from an array (using filter, using Set Object).](#QA3)
- [Shuffle elements in an array.](#QA4)
- [Find average of an array.](#QA5)
- [Use javascript function to perform a quick sort.](#QA6)
- [Flatten the array using ES6 functions and find unique numbers.](#QA7)
```
Input: array1 = [[1, 2], [3, 4], [4, 6], [2, 5]];
Output: [1, 2, 3, 4, 5, 6]
```
- [Find longest common string from array of strings](#QA8)
```
Input: array1 = ["go","google","gosh"];
Output: "go"
```
- [Unique values only from 2 arrays](#QA9)
```
Input: array1 = [1,2,3,4]; array2 = [2,3,4,5];
Output: [1,5]
```
- [Find the first pair whose sum is 0](#QA10)
```
Input: array1 = [-5,-4,-3,-2,-1,0,1,2,3,4,5];
Output: 
```
- [Find fibonacci series](#QA11)
- [Find missing number in an array](#QA12)
- [Find unique numbers from 2 arrays and keep it in one array](#QA13)
- [Write a program that prints the numbers from 1 to 100. But for multiples of three, print "Fizz" instead of the number, and for the multiples of five, print "Buzz". For numbers which are multiples of both three and five, print "FizzBuzz"](#QA14)
- [Uppercase of each first letter of a words](#QA15)
- [Find the largest elements fro the 2 diensional array](#QA16)
- [Converting one dimensional array into n dimensional array using splice](#QA17)
- [Find only truthy values](#QA18)
- [Checking all letters of second words should present in first word, in the same order using include function](#QA19)

## Strings
- [Given a string, reverse each word in the sentence. Example "emocleW ot aidnI". Return as "Welcome to India"](#QB1)
- [Given two strings, return true if they are anagrams of one another.](#QB2)
- [Find a maximum consecutive repeating char in a given string.](#QB3)
- [Remove duplicate characters from a string](#QB4)
```
Input: string = 'india is unique'
Output: 'indasuqe'
```
- [String reverse without reversing of individual words (using inbuilt function, not using inbuilt function)](#QB5)
```
Input: string = 'India is my country'
Output: 'aidnI si ym yrtnuoc'
```
- [Check anagram](#QB6)
```
Input: a = 'Army'; b = 'Mary
Output: true
```
- [Check palindrome (using inbuilt function, not using inbuilt function).](#QB7)
```
Input: string = 'anmna'
Output: true
```
- [Find the longest word from the string using for-of loop](#QB8)
```
Input: string = 'supriya is a masooooom good girl'
Output: 'masooooom'
```
- [Find vowels and its count in a given string](#QB9)
- [Find character occurance fro the string](#QB10)
- [Check ending of the string with given character/s (using inbuilt function, not using inbuilt function).](#QB11)

## Objects
- [Check if a given object is empty or not.](#QC1)

## Recursion
- [Write a function for factorial program.](#QD1)

## Binary Search

## JavaScript General
- [Output of the following.](#QE1)
```
console.log('one');
setTimeout(() => console.log('two'));
console.log('three');0
```

# Answers
#### QA1 
### ✍Write a function to remove duplicates in an array, sort it in the descending order.
<details><summary><b>Answer</b></summary>

```js
const arr = [5, 2, 7, 5, 8, 4, 7, 2];
let output = [];
for (i = 0; i < arr.length; i++) {
   if(output.indexOf(arr[i]) == -1) {
       output.push(arr[i]);
   }
}
console.log(output.sort((a, b) => { return b-a }));
```
</details>

**[⬆](#Questions)**
---
#### QA2
### ✍How to empty an array.

**[⬆](#Questions)**
---
#### QA3
### ✍Remove duplicate values from an array (using filter, using Set Object).

**[⬆](#Questions)**
---
#### QA4
### ✍Shuffle elements in an array.

**[⬆](#Questions)**
---
#### QA5
### ✍Find average of an array.
<details><summary><b>Answer</b></summary>

```js
const numbers = [1, 2, 3, 4, 5];

const getAverage = (array) => (array.reduce((total, current) => {
	return total + current;
}, 0)) / array.length;

console.log(getAverage(numbers)); // 3
```
</details>

**[⬆](#Questions)**
---
#### QA6
### ✍Use javascript function to perform a quick sort.
<details><summary><b>Answer</b></summary>

```js
function quickSort(arr) {
    if (arr.length <= 1) return arr;

    const newArr = arr.slice();
    let pivot = newArr[0];
    const left = [];
    const right = [];

    // start from index 1 as we're taking the first element as pivot
    for (let i = 1; i < newArr.length; i++) {
        newArr[i] < pivot ? left.push(newArr[i]) : right.push(newArr[i]);
    }

    return [...quickSort(left), pivot, ...quickSort(right)];
}

const numbers = [5, 3, 7, 6, 2, 9];
console.log(quickSort(numbers)); // [2, 3, 5, 6, 7, 9]
```
</details>

---
#### QA7
### ✍Flatten the array using ES6 functions and find unique numbers.
<details><summary><b>Answer</b></summary>

```js

```
</details>

---
#### QA8
### ✍Find longest common string from array of strings
<details><summary><b>Answer</b></summary>

```js

```
</details>

---
#### QA9
### ✍Unique values only from 2 arrays
<details><summary><b>Answer</b></summary>

```js

```
</details>

---
#### QA10
### ✍Find the first pair whose sum is 0
<details><summary><b>Answer</b></summary>

```js

```
</details>

---
#### QA11
### ✍Find fibonacci series
<details><summary><b>Answer</b></summary>

```js

```
</details>

---
#### QA12
### ✍Find missing number in an array
<details><summary><b>Answer</b></summary>

```js

```
</details>

---
#### QA13
### ✍Find unique numbers from 2 arrays and keep it in one array
<details><summary><b>Answer</b></summary>

```js

```
</details>

---
#### QA14
### ✍Write a program that prints the numbers from 1 to 100. But for multiples of three, print "Fizz" instead of the number, and for the multiples of five, print "Buzz". For numbers which are multiples of both three and five, print "FizzBuzz"
<details><summary><b>Answer</b></summary>

```js

```
</details>

---
#### QA15
### ✍Uppercase of each first letter of a words
<details><summary><b>Answer</b></summary>

```js

```
</details>

---
#### QA16
### ✍Find the largest elements fro the 2 diensional array
<details><summary><b>Answer</b></summary>

```js

```
</details>

---
#### QA17
### ✍Converting one dimensional array into n dimensional array using splice
<details><summary><b>Answer</b></summary>

```js

```
</details>

---
#### QA18
### ✍Find only truthy values.
<details><summary><b>Answer</b></summary>

```js

```
</details>

---
#### QA19
### ✍Checking all letters of second words should present in first word, in the same order using include function.
<details><summary><b>Answer</b></summary>

```js

```
</details>

**[⬆](#Questions)**
---
#### QB1
### ✍Given a string, reverse each word in the sentence. Example ""emocleW ot aidnI". Return as "Welcome to India".
<details><summary><b>Answer</b></summary>

```js
let str = "emocleW ot aidnI";

let arr = str.split(' ');

let result = arr.map((item) => {
	return item.split('').reverse().join('');
});

console.log(result.join(' ')); // "Welcome to India"
```
</details>

**[⬆](#Questions)**
---
#### QB2
### ✍Given two strings, return true if they are anagrams of one another. 
<details><summary><b>Answer</b></summary>

```js
let strA = "monk";
let strB = "kmon";

function checkString(str) {
	return str.replace(/[^\w]/g).toLowerCase().split('').sort().join();
}

function isAnagram(strA, strB) {
	return checkString(strA) === checkString(strB);
}

console.log(isAnagram(strA, strB)); // true
```
</details>

**[⬆](#Questions)**
---
#### QB3
### ✍Find a maximum consecutive repeating char in a given string.
<details><summary><b>Answer</b></summary>

```js
/* Find occurance of each letter */
let str = "emocleW ot aidnI";

let replacedStr = str.replaceAll(' ', '');

// Method 1 - Using for loop
/* const resultObj = {};
let char, count;

for(let i = 0; i < replacedStr.length; i++) {
  char = replacedStr.charAt(i);

  resultObj[char] = count ? count + 1 : 1; 
} */

// Method 2 - Using reduce()
let result = [...replacedStr].reduce((total, curr) => {
	total[curr] = total[curr] ? total[curr] + 1 : 1;
    return total;
}, {});

console.log(result);
// {
//   a: 1,
//   c: 1,
//   d: 1,
//   e: 2,
//   i: 1,
//   I: 1,
//   l: 1,
//   m: 1,
//   n: 1,
//   o: 2,
//   t: 1,
//   W: 1
// }
```
</details>

---
#### QB4
### ✍Remove duplicate characters from a string
<details><summary><b>Answer</b></summary>

```js

```
</details>

---
#### QB5
### ✍String reverse without reversing of individual words (using inbuilt function, not using inbuilt function)
<details><summary><b>Answer</b></summary>

```js

```
</details>

---
#### QB6
### ✍Check anagram
<details><summary><b>Answer</b></summary>

```js

```
</details>

---
#### QB7
### ✍Check palindrome (using inbuilt function, not using inbuilt function).
<details><summary><b>Answer</b></summary>

```js

```
</details>

---
#### QB8
### ✍Find the longest word from the string using for-of loop
<details><summary><b>Answer</b></summary>

```js

```
</details>

---
#### QB9
### ✍Find vowels and its count in a given string
<details><summary><b>Answer</b></summary>

```js

```
</details>

---
#### QB10
### ✍Check ending of the string with given character/s (using inbuilt function, not using inbuilt function).
<details><summary><b>Answer</b></summary>

```js

```
</details>

**[⬆](#Questions)**
---
#### QC1
### ✍Check if a given object is empty or not.

**[⬆](#Questions)**
---
#### QD1
### ✍Write a function for factorial program.
<details><summary><b>Answer</b></summary>

```js
let factorial = function(n) {
    if(n <= 0) {
        return 1;
    } else {
        return n * factorial(n-1);
    }
}
var result = factorial(6);
console.log(result);
```
</details>

**[⬆](#Questions)**
---
#### QE1
### ✍Output of the following.
<details><summary><b>Answer</b></summary>

```js
console.log('one');
setTimeout(() => console.log('two'));
console.log('three');0

// RESULT: 
// one
// three
// two
```
</details>

