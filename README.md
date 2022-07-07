# javascript-notes-problem-solving


1. Print in Console numbers from 1 to 10
2. Print in Console the odd numbers less than 100
3. Print in Console the multiplication table with 7
4. Calculate the sum of numbers from 1 to 10
5. Calculate 10!
6. Calculate the sum of odd numbers greater than 10 and less than 30
7. Calculate the sum of numbers in an array of numbers
8. Calculate the average of the numbers in an array of numbers
9. Find the maximum number in an array of numbers
10. Create a function that receives an array of numbers and returns an array containing only the positive numbers
11. Print in Console all the multiplication tables with numbers from 1 to 10
12. Create a function that will convert from Celsius to Fahrenheit
13. Create a function that will convert from Fahrenheit to Celsius
14. Print in Console the first 10 Fibonacci numbers without recursion
15. Create a function that will find the nth Fibonacci number using recursion
16. Check Leap Year Using if...else?
17. Create a function that accepts an array and returns the last item in the array.
18. Calculate the sum of digits of a positive integer number
19. Print in Console the first 100 prime numbers
20. Check Odd or Even Number with Arguments Objects
21. Create a function that will return in an array the first "nPrimes" prime numbers greater than a particular number "startAt"
22. Rotate an array to the left 1 position
23. Reverse an array with createed function, don`t Change orginal array #24: Reverse an array with JavaScript Builtin Method
24. Reverse a string with JavaScript Builtin Method
25. Reverse a string with createed function, don`t Change orginal string
26. Create a function that takes an array and returns the types of values (data types) in a new array.
27. Create a function that will return in an array. becarefull function parameter and array length is same in count.
28. Create a function that takes the age in years and returns the age in days.
29. Create a function that takes voltage and current and returns the calculated power.
30. Given two numbers, return true if the sum of both numbers is less than 50. Otherwise return false.
31. Write a function that takes minutes and converts it to seconds.
32. Write a function that converts hours into seconds.
33. Create a function that takes an array containing only numbers and return the first element.
34. Create a function that finds the maximum range of a triangle's third edge, where the side lengths are all integers.
35. Write a function that takes the base and height of a triangle and return its area.
36. Create a function that takes a number as an argument, increments the number by +1 and returns the result.
37. Create a function that takes a base number and an exponent number and returns the calculation.
38. Create a function that takes two numbers as arguments and return their sum.
39. Create a function that will merge two arrays and return the result as a new array
40. Create a function that will receive two arrays of numbers as arguments and return an array composed of all the numbers that are either in the first array or second array but not in both

**#1: Print in Console from 1 to 10 numbers?**

```js

for (let i = 1; i <= 10; i++) {
  console.log(i);
}

```

**#2: Print in Console the odd numbers less than 100?**

```js

for (let i = 1; i <= 100; i += 2) {
  console.log(i);
}

```

**#3: Print in Console the multiplication table with 7?**

```js

for (let i = 1; i <= 10; i++) {
  console.log(`7 x ${i} = ${i * 7}`);
}

```

**#4: Calculate the sum of numbers from 1 to 10?**

```js

let sum = 0;
for (let i = 1; i <= 10; i++) {
  sum += i;
}
console.log(sum);

```

**#5: Calculate 10!?**

```js

let fabCalculate = 1;
for (let i = 1; i <= 10; i++) {
  fabCalculate *= i;
}
console.log(fabCalculate);

```

**#6: Calculate the sum of odd numbers greater than 10 and less than 30?**

```js

let sumOdd = 0;
for (let i = 10; i <= 30; i += 2) {
  sumOdd += i;
}
console.log(sumOdd);

```

**#7: Calculate the sum of numbers in an array of numbers?**

```js

let arr = [50, 67, 20, 84, 91, 40, 69];
let arrTotal = 0;
for (let i = 0; i < arr.length; i++) {
  arrTotal += arr[i];
}
console.log(arrTotal);

```

**#8: Calculate the average of the numbers in an array of numbers?**

```js

const arrAverage = (arr) => {
  let arrTotal = 0;
  for (let i = 0; i < arr.length; i++) {
    arrTotal += arr[i];
  }
  return arrTotal / arr.length;
};
console.log(arrAverage(arr));

```

**#9: Find the maximum number in an array of numbers?**

```js

const findMaxNumber = (arr) => Math.max(...arr);

console.log(findMaxNumber(arr));

```

**#10: Create a function that receives an array of numbers and returns an array containing only the positive numbers?**

```js

const getPositiveNumber = (arr) => {
  const newArr = [];
  for (let i = 0; i < arr.length; i++) {
    if (arr[i] % 2 == 0) {
      newArr.push(arr[i]);
    }
  }
  return newArr;
};
console.log(getPositiveNumber(arr));

```

**#11: Print in Console all the multiplication tables with numbers from 1 to 10?**

```js

const printMultiplicationTable = (n) => {
  for (let i = 1; i <= n; i++) {
    for (let j = 1; j <= 10; j++) {
      console.log(`${i} x ${j} = ${i * j}`);
    }
  }
};
printMultiplicationTable(10);

```

**#12: Create a function that will convert from Celsius to Fahrenheit?**

```js

const celsiustoFahrenheit = (n) => n * 1.8 + 32;
console.log(celsiustoFahrenheit(50));

```

**#13: Create a function that will convert from Fahrenheit to Celsius?**

```js

const fahrenheittoCelsius = (n) => ((n - 32) * 5) / 9;
console.log(fahrenheittoCelsius(50));

```

**#14: Create a function that will find the nth Fibonacci number using recursion?**

```js

function findFibonacci(n) {
  if (n == 0) return 0;

  if (n == 1) return 1;

  return findFibonacci(n - 1) + findFibonacci(n - 2);
}
console.log(findFibonacci(20));

```

**#15: Create a function that will return a Boolean specifying if a number is prime?**

```js

function isPrime(num) {
  for (var i = 2; i < num; i++)
    if (num % i === 0) {
      return num < 1;
    }
  return num > 1;
}
console.log(isPrime(6));

```

**#16: Check Leap Year Using if...else?**

```js

function checkLeapYear(year) {
  if ((year % 4 == 0 && year % 100 != 0) || year % 400 == 0) {
    return year > 1;
  } else {
    return year < 1;
  }
}
console.log(checkLeapYear(2025));

```

**#17: Create a function that accepts an array and returns the last item in the array?**

```js

const arr = [50, 90, 80, 66, 85];
const returnLastItem = (arr) => arr[arr.length - 1];
console.log(returnLastItem(arr));

```

**#18: Calculate the sum of digits of a positive integer number?**

```js

const sumOfDigits = (n) => {
  const newArr = Array.from(String(n), Number);
  let sumOfArr = 0;
  for (let i = 0; i < newArr.length; i++) {
    sumOfArr += newArr[i];
  }
  return sumOfArr;
};
console.log(sumOfDigits(45465));

```

**#19: Print in Console the first 50 prime numbers**

```js

getPrime(50);
function getPrime(nPrime) {
  let prime = 1;
  for (let i = 2; prime <= nPrime; i++) {
    if (isPrime(i)) {
      console.log(prime, " ", i);
      prime++;
    }
  }
}

function isPrime(num) {
  for (var i = 2; i < num; i++)
    if (num % i === 0) {
      return num < 1;
    }
  return num > 1;
}

```

**#20: Check Odd or Even Number with Arguments Objects**

```js

function checkOddOrEven() {
  for (let i = 0; i < arguments.length; i++) {
    arguments[i] % 2 == 0
      ? console.log(arguments[i] + " is Even Number")
      : console.log(arguments[i] + " is Odd Number");
  }
}
checkOddOrEven(11, 10, 20);

```

**#21: Create a function that will return in an array the first "nPrimes" prime numbers greater than a particular number "startAt**

```js

console.log(getFirstNprimeNumber(5, 500));
function getFirstNprimeNumber(nPrimes, startAt) {
  const arr = [];
  for (let i = startAt; arr.length < nPrimes; i++) {
    if (isPrime(i)) {
      arr.push(i);
    }
  }
  return arr;
}
function isPrime(num) {
  for (var i = 2; i < num; i++)
    if (num % i === 0) {
      return num < 1;
    }
  return num > 1;
}

```

**#22: Rotate an array to the left 1 position**

```js

const arr = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12];

rotateLeft(arr);
function rotateLeft(arr) {
  const arrFirstElement = arr.shift();
  arr.push(arrFirstElement);
}
console.log(arr);

```

**#23: Reverse an array with createed function, don`t Change orginal array**

```js

const arr = [1, 2, 3];

const newArr = reverseArr(arr);
console.log(newArr);

function reverseArr(arr) {
const newArr = [];
for (let i = arr.length - 1; i >= 0; i--) {
newArr.push(arr[i]);
}
return newArr;
}


```

**#24: Reverse an array with JavaScript Builtin Method**

```js

const arr = [1, 2, 3];
arr.reverse();
console.log(arr);

```

**#25: Reverse a string with createed function, don`t Change orginal string**

```js

const str = "Md Nazmul Islam";

const newStr = reverseString(str);
console.log(newStr);

function reverseString(str) {
  let newStr = "";
  for (let i = str.length - 1; i >= 0; i--) {
    newStr += str[i];
  }
  return newStr;
}

```

**#26: Reverse a string with JavaScript Builtin Method**

```js

const str = "Md Nazmul islam";
const newStr = str.split("").reverse().join("");
console.log(newStr);

```

**#27: Create a function that takes an array and returns the types of values (data types) in a new array.**

```js

const arrayValuesTypes = (arr) => {
  const newArr = [];
  for (let i = 0; i < arr.length; i++) {
    newArr.push(typeof arr[i]);
  }
  return newArr;
};
console.log(arrayValuesTypes([1, 2, "Nazmul", [], true]));

```

**Or ShortCut**

```js

const arrayValuesTypes = (arr) => arr.map((x) => typeof x);
console.log(arrayValuesTypes([1, 2, "Nazmul", [], true]));

```

**#28: Create a function that will return in an array. becarefull function parameter and array length is same in count.**

```js

function getArray(number) {
  var newArray = [];
  for (var i = 1; i <= number; i++) {
    newArray.push(i);
  }
  return newArray;
}
console.log(getArray(5));

```

**Or ShortCut**

```js

const getArray = (n) => Array(...Array(n)).map((v, i) => i + 1);
console.log(getArray(5));

```

**#29: Create a function that takes the age in years and returns the age in days.**

```js

const calcAge = (age) => (age < 0 || typeof age != "number" ? null : age * 365);
console.log(calcAge(5));

```

**#30: Create a function that takes voltage and current and returns the calculated power.**

```js

const circuitPower = (voltage, current) => voltage * current;
console.log(circuitPower(115, 5));

```

**#31: Given two numbers, return true if the sum of both numbers is less than 50. Otherwise return false.**

```js

function lessThan50(a, b) {
  if (a + b < 50) {
    return true;
  } else {
    return false;
  }
}
console.log(lessThan50(40, 30));

```

**Or ShortCut**

```js

const lessThan50 = (a, b) => a + b < 50;
console.log(lessThan50(30.15));

```

**#32: Write a function that takes minutes and converts it to seconds.**

```js

const minuteToSecond = (minutes) => minutes * 60;
console.log(minuteToSecond(2));

```

**#33: Write a function that converts hours into seconds.**

```js

const hoursToSeconds = (hours) => hours * 60 * 60;
console.log(hoursToSeconds(2));

```

**#34: Create a function that takes an array containing only numbers and return the first element.**

```js

const getFirstValueOfArray = (arr) => arr[0];

```

**#35: Create a function that finds the maximum range of a triangle's third edge, where the side lengths are all integers.**

```js

const nextEdge = (side1, side2) => side1 + side2 - 1;

```

**#36: Write a function that takes the base and height of a triangle and return its area.**

```js

const triangleArea = (base, height) => (base * height) / 2;

```

**#37: Create a function that takes a number as an argument, increments the number by +1 and returns the result.**

```js

const incrementsNumber = (n) => ++n;

```

**#38: Create a function that takes a base number and an exponent number and returns the calculation.**

```js

const calculateExponent = (num, exp) => Math.pow(num, exp);

```

**#39: Create a function that takes two numbers as arguments and return their sum.**

```js

function addition(a, b) {
  if (typeof a !== "number" || typeof b !== "number") {
    return "Sorry you didn't pass two numbers.";
  }
  return a + b;
}

```

**#40: Create a function that will merge two arrays and return the result as a new array**

```js

const mergeArrays = (arr1, arr2) => {
  return [...arr1, ...arr2];
};
console.log(mergeArrays([5, 3, 6], [8, 7]));

```

**// Or**

```js

function mergeArrays(arr1, arr2) {
  var arr = [];

  for (let element of arr1) {
    arr.push(element);
  }

  for (let element of arr2) {
    arr.push(element);
  }

  return arr;
}
console.log(mergeArrays([5, 3, 6], [8, 7]));

```
