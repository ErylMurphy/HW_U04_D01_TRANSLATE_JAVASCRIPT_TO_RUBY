# Ruby Monk and Translate JavaScript to Ruby Lab

## Part 1: 
Work through the [RubyMonk Primer](http://rubymonk.com/learning/books/1-ruby-primer) from “Classes and Object Oriented Programming in Ruby”  to “Introduction to Lambdas and Blocks”.

## Part 2:

### Let's Look at the Differences

![cat owls](https://outofdoubt.files.wordpress.com/2015/01/not-like-the-others-owls.jpg)

## Rewrite the following Javascript functions in Ruby

### Get Name
```javascript
var getName = function () {
  var name = prompt("what is your name?");
  return name;
};
```

### Reverse It
```javascript
var reverseIt = function () {
  var string = "a man, a plan, a canal, frenemies!";

  var reverse = "";

  for (var i=0; i < string.length; i++) {
    reverse += string[string.length - (i+1)];
  };

  alert(reverse);
};
```
### Swap Em
```javascript
var swapEm = function () {
  var a = 10;
  var b = 30;
  var temp;

  temp = b;
  b = a;
  a = temp;

  alert("a is now " + a + ", and b is now " + b);
};
```
### Multiply Array
```javascript
var multiplyArray = function (ary) {
  if (ary.length == 0) { return 1; };

  var total = 1;
  // var total = ary[0];

  for (var i=0; i < ary.length; i++) {
    total = total * ary[i];
  };

  return total;
};
```

### Array includes a value
``` javascript
var searchArray = function(array,value) {
  for(var i = 0; i < array.length-1; i++) {
    if(array[i] == value) {
      return true;
      break;
    }
  }
  return -1;
};
```
## Bonuses:

### Nth Fibonacci Number
```javascript
var nthFibonacciNumber = function () {
  var fibs = [1, 1];
  var num = prompt("which fibonacci number do you want?");

  while (fibs.length < parseInt(num)) {
    var length = fibs.length;
    var nextFib = fibs[length - 2] + fibs[length - 1];
    fibs.push(nextFib);
  }

  alert(fibs[fibs.length - 1] + " is the fibonacci number at position " + num);
};
```

### Palindrome
``` javascript
var isPalindrome = function(str) {
  for(var i = 0; i < str.length/2; i++){
    if(str[i] != str[str.length-i-1]){
      return false;
      break;
    }
    return true;
  }
};
```

### hasDupes
``` javascript
var hasDupes = function(arr){
  var obj = {};
  for (i = 0; i < arr.length; i++) {
    if(obj[arr[i]]) {
      return true;
    }
    else {
      obj[arr[i]] = true;
    }
  }
  return false;
};
```

## Sign up for Code Wars
Pick some Ruby code challenges, find a good one? Share it in slack!
