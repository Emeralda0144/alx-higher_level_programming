# 0x12. JavaScript - Warm up

`JavaScript`

### Background Context
JavaScript is used for many things. Here, you will use JavaScript for 2 reasons:

* Scripting (same as we did with Python)
* Web front-end

For the moment, and for learning all basic concepts of this language, we will do some scripting. After, we will make our AirBnB project dynamic by using Javascript and JQuery.

![](https://s3.amazonaws.com/intranet-projects-files/holbertonschool-higher-level_programming+/303/Javascript-535.png.jpeg)

## Resources
**Read or watch:**

* Writing JavaScript Code
* Variables
* Data Types
* Operators
* Operator Precedence
* Controlling Program Flow
* Functions
* Objects and Arrays
* Intrinsic Objects
* Module patterns
* var, let and const
* JavaScript Tutorial
* Modern JS]()

# Learning Objectives

* Why JavaScript programming is amazing
* How to run a Javascript script
* How to create variables and constants
* What are differences between `var`, `const` and `let`
* What are all the data types available in Javascript
* How to use the `if`, `if ... else` statements
* How to use comments
* How to affect values to variables
* How to use `while` and `for` loops
* How to use `break` and `continue` statements
* What is a function and how do you use functions
* What does a function that does not use any `return` statement return
* Scope of variables
* What are the arithmetic operators and how to use them
* How to manipulate dictionary
* How to import a file

## Requirements

### General
* Allowed editors: `vi`, `vim`, `emacs`
* All your files will be interpreted on Ubuntu 20.04 LTS using `node` (version 14.x)
* All your files should end with a new line
* The first line of all your files should be exactly `#!/usr/bin/node`
* A `README.md` file, at the root of the folder of the project, is mandatory
* Your code should be `semistandard` compliant (version 16.x.x). [Rules of Standard]() + [semicolons on top](https://github.com/standard/semistandard). Also as reference: [AirBnB style](https://github.com/airbnb/javascript)
* All your files must be executable
* The length of your files will be tested using `wc`

## More Info

### Install Node 14
```
$ curl -sL https://deb.nodesource.com/setup_14.x | sudo -E bash -
$ sudo apt-get install -y nodejs
```
### Install semi-standard
[Documentation](https://intranet.alxswe.com/rltoken/35q5Pc6A6KWPyd3kGeRQFg)
```
$ sudo npm install semistandard --global
```

## Tasks

### 0. First constant, first print
Write a script that prints “Javascript is amazing”:

* You must create a constant variable called `myVar` with the value “Javascript is amazing”
* You must use `console.log(...)` to print all output
* You are not allowed to use `var`

**Solution:** [0-javascript_is_amazing.js](https://github.com/Emeralda0144/alx-higher_level_programming/blob/master/0x12-javascript-warm_up/0-javascript_is_amazing.js)

```
$ guillaume@ubuntu:~/0x12$ ./0-javascript_is_amazing.js 
Javascript is amazing
$ guillaume@ubuntu:~/0x12$ 
$ guillaume@ubuntu:~/0x12$ semistandard ./0-javascript_is_amazing.js 
$ guillaume@ubuntu:~/0x12$
```

### 1. 3 languages
Write a script that prints 3 lines:

* The first line: “C is fun”
* The second line: “Python is cool”
* The third line: “Javascript is amazing”
* You must use `console.log(...)` to print all output
* You are not allowed to use `var`

**Solution:** [1-multi_languages.js](https://github.com/Emeralda0144/alx-higher_level_programming/blob/master/0x12-javascript-warm_up/1-multi_languages.js)

```
$ guillaume@ubuntu:~/0x12$ ./1-multi_languages.js 
C is fun
Python is cool
Javascript is amazing
$ guillaume@ubuntu:~/0x12$
```

## 2. Arguments
Write a script that prints a message depending of the number of arguments passed:

* If no arguments are passed to the script, print “No argument”
* If only one argument is passed to the script, print “Argument found”
* Otherwise, print “Arguments found”
* You must use `console.log(...)` to print all output
* You are not allowed to use `var`

**Solution:** [2-arguments.js](https://github.com/Emeralda0144/alx-higher_level_programming/blob/master/0x12-javascript-warm_up/2-arguments.js)

```
$ guillaume@ubuntu:~/0x12$ ./2-arguments.js 
No argument
$ guillaume@ubuntu:~/0x12$ ./2-arguments.js Holberton
Argument found
$ guillaume@ubuntu:~/0x12$ ./2-arguments.js Holberton School
Arguments found
$ guillaume@ubuntu:~/0x12$
```

## 3. Value of my argument
Write a script that prints the first argument passed to it:

* If no arguments are passed to the script, print “No argument”
* You must use `console.log(...)` to print all output
* You are not allowed to use `var`
* You are not allowed to use `length`

**Solution:** [3-value_argument.js](https://github.com/Emeralda0144/alx-higher_level_programming/blob/master/0x12-javascript-warm_up/3-value_argument.js)

```
$ guillaume@ubuntu:~/0x12$ ./3-value_argument.js 
No argument
$ guillaume@ubuntu:~/0x12$ ./3-value_argument.js Holberton
Holberton
$ guillaume@ubuntu:~/0x12$
```

### 4. Create a sentence
Write a script that prints two arguments passed to it, in the following format: “ is ”

* You must use `console.log(...)` to print all output
* You are not allowed to use `var`

**Solution:** [4-concat.js](https://github.com/Emeralda0144/alx-higher_level_programming/blob/master/0x12-javascript-warm_up/4-concat.js)

```
$ guillaume@ubuntu:~/0x12$ ./4-concat.js c cool
c is cool
$ guillaume@ubuntu:~/0x12$ ./4-concat.js c 
c is undefined
$ guillaume@ubuntu:~/0x12$ ./4-concat.js
undefined is undefined
$ guillaume@ubuntu:~/0x12$
```

### 5. An Integer
Write a script that prints `My number: <first argument converted in integer>` if the first argument can be converted to an integer:

* If the argument can’t be converted to an integer, print “Not a number”
* You must use `console.log(...)` to print all output
* You are not allowed to use `var`
* You are not allowed to use `try/catch`

**Solution:** [5-to_integer.js](https://github.com/Emeralda0144/alx-higher_level_programming/blob/master/0x12-javascript-warm_up/5-to_integer.js)

```
$ guillaume@ubuntu:~/0x12$ ./5-to_integer.js 
Not a number
$ guillaume@ubuntu:~/0x12$ ./5-to_integer.js 89
My number: 89
$ guillaume@ubuntu:~/0x12$ ./5-to_integer.js "89"
My number: 89
$ guillaume@ubuntu:~/0x12$ ./5-to_integer.js 89.89
My number: 89
$ guillaume@ubuntu:~/0x12$ ./5-to_integer.js Holberton
Not a number
$ guillaume@ubuntu:~/0x12$
```

### 6. Loop to languages
Write a script that prints 3 lines: (like `1-multi_languages.js`) but by using an array of string and a loop

* The first line: “C is fun”
* The second line: “Python is cool”
* The third line: “Javascript is amazing”
* You must use `console.log(...)` to print all output
* You are not allowed to use `var`
* You are not allowed to use any `if/else` statement
* You can use only one `console.log`
* You must use a loop (`while`, `for`, etc.)

**Solution:** [6-multi_languages_loop.js](https://github.com/Emeralda0144/alx-higher_level_programming/blob/master/0x12-javascript-warm_up/6-multi_languages_loop.js)

```
$ guillaume@ubuntu:~/0x12$ ./6-multi_languages_loop.js 
C is fun
Python is cool
Javascript is amazing
$ guillaume@ubuntu:~/0x12$
```

### 7. I love C
Write a script that prints `x` times “C is fun”

* Where `x` is the first argument of the script
* If the first argument can’t be converted to an integer, print “Missing number of occurrences”
* You must use `console.log(...)` to print all output
* You are not allowed to use `var`
* You can use only two `console.log`
* You must use a loop (`while`, `for`, etc.)

**Solution:** [7-multi_c.js](https://github.com/Emeralda0144/alx-higher_level_programming/blob/master/0x12-javascript-warm_up/7-multi_c.js)

```
$ guillaume@ubuntu:~/0x12$ ./7-multi_c.js 2
C is fun
C is fun
$ guillaume@ubuntu:~/0x12$ ./7-multi_c.js 5
C is fun
C is fun
C is fun
C is fun
C is fun
$ guillaume@ubuntu:~/0x12$ ./7-multi_c.js 
Missing number of occurrences
$ guillaume@ubuntu:~/0x12$ ./7-multi_c.js -3
$ guillaume@ubuntu:~/0x12$
```

### 8. Square
Write a script that prints a square

* The first argument is the size of the square
* If the first argument can’t be converted to an integer, print “Missing size”
* You must use the character `X` to print the square
* You must use `console.log(...)` to print all output
* You are not allowed to use `var`
* You must use a loop (`while`, `for`, etc.)

**Solution:** [8-square.js](https://github.com/Emeralda0144/alx-higher_level_programming/blob/master/0x12-javascript-warm_up/8-square.js)

```
$ guillaume@ubuntu:~/0x12$ ./8-square.js
Missing size
$ guillaume@ubuntu:~/0x12$ ./8-square.js Holberton
Missing size
$ guillaume@ubuntu:~/0x12$ ./8-square.js 2
XX
XX
$ guillaume@ubuntu:~/0x12$ ./8-square.js 6
XXXXXX
XXXXXX
XXXXXX
XXXXXX
XXXXXX
XXXXXX
$ guillaume@ubuntu:~/0x12$ ./8-square.js -3
$ guillaume@ubuntu:~/0x12$
```

### 9. Add
Write a script that prints the addition of 2 integers

* The first argument is the first integer
* The second argument is the second integer
* You have to define a function with this prototype: `function add(a, b)`
* You must use `console.log(...)` to print all output
* You are not allowed to use `var`

**Solution:** [9-add.js](https://github.com/Emeralda0144/alx-higher_level_programming/blob/master/0x12-javascript-warm_up/9-add.js)

```
$ guillaume@ubuntu:~/0x12$ ./9-add.js 
NaN
$ guillaume@ubuntu:~/0x12$ ./9-add.js 1
NaN
$ guillaume@ubuntu:~/0x12$ ./9-add.js 1 7
8
$ guillaume@ubuntu:~/0x12$ ./9-add.js 13 89
102
$ guillaume@ubuntu:~/0x12$
```

### 10. Factorial
Write a script that computes and prints a factorial

* The first argument is integer (argument can be cast as integer) used for computing the factorial
* Factorial of `NaN` is `1`
* You must do it recursively
* You must use a function
* You must use `console.log(...)` to print all output
* You are not allowed to use `var`

**Solution:** [10-factorial.js](https://github.com/Emeralda0144/alx-higher_level_programming/blob/master/0x12-javascript-warm_up/10-factorial.js)

```
$ guillaume@ubuntu:~/0x12$ ./10-factorial.js 
1
$ guillaume@ubuntu:~/0x12$ ./10-factorial.js 3
6
$ guillaume@ubuntu:~/0x12$ ./10-factorial.js 89
1.6507955160908452e+136
$ guillaume@ubuntu:~/0x12$ ./10-factorial.js 333
Infinity
$ guillaume@ubuntu:~/0x12$
```

## 11. Second biggest!
Write a script that searches the second biggest integer in the list of arguments.

* You can assume all arguments can be converted to integer
* If no argument passed, print `0`
* If the number of arguments is 1, print `0`
* You must use `console.log(...)` to print all output
* You are not allowed to use `var`

**Solution:** [11-second_biggest.js](https://github.com/Emeralda0144/alx-higher_level_programming/blob/master/0x12-javascript-warm_up/11-second_biggest.js)

```
$ guillaume@ubuntu:~/0x12$ ./11-second_biggest.js 
0
$ guillaume@ubuntu:~/0x12$ ./11-second_biggest.js 1
0
$ guillaume@ubuntu:~/0x12$ ./11-second_biggest.js 4 2 5 3 0 -3
4
$ guillaume@ubuntu:~/0x12$
```

### 12. Object
Update this script to replace the value `12` with `89`:

* You are not allowed to use `var`

**Solution:** [12-object.js](https://github.com/Emeralda0144/alx-higher_level_programming/blob/master/0x12-javascript-warm_up/12-object.js)

```
$ guillaume@ubuntu:~/0x12$ cat 12-object.js
#!/usr/bin/node
const myObject = {
  type: 'object',
  value: 12
};
console.log(myObject);
/*
YOUR CODE HERE
*/
console.log(myObject);

$ guillaume@ubuntu:~/0x12$ ./12-object.js
{ type: 'object', value: 12 }
{ type: 'object', value: 89 }
$ guillaume@ubuntu:~/0x12$
```

### 13. Add file
Write a function that returns the addition of 2 integers.

* The function must be visible from outside
* The name of the function must be `add`
* You are not allowed to use `var`

**Solution:** [13-add.js](https://github.com/Emeralda0144/alx-higher_level_programming/blob/master/0x12-javascript-warm_up/13-add.js)

```
$ guillaume@ubuntu:~/0x12$ cat 13-main.js
#!/usr/bin/node
const add = require('./13-add').add;
console.log(add(3, 5));
$ guillaume@ubuntu:~/0x12$ ./13-main.js
8
$ guillaume@ubuntu:~/0x12$
```

### 14. Const or not const
Write a file that modifies the value of `myVar` to `333`

**Solution:** [100-let_me_const.js](https://github.com/Emeralda0144/alx-higher_level_programming/blob/master/0x12-javascript-warm_up/100-let_me_const.js)

```
$ guillaume@ubuntu:~/0x12$ cat 100-main.js
#!/usr/bin/node
myVar = 89;
require('./100-let_me_const')
console.log(myVar);
$ guillaume@ubuntu:~/0x12$ ./100-main.js
333
$ guillaume@ubuntu:~/0x12$
```

### 15. Call me Moby
Write a function that executes `x` times a function.

* The function must be visible from outside
* Prototype: `function (x, theFunction)`
* You are not allowed to use `var`

**Solution:** [101-call_me_moby.js](https://github.com/Emeralda0144/alx-higher_level_programming/blob/master/0x12-javascript-warm_up/101-call_me_moby.js)

```
$ guillaume@ubuntu:~/0x12$ cat 101-main.js
#!/usr/bin/node
const callMeMoby = require('./101-call_me_moby').callMeMoby;
callMeMoby(3, function () {
  console.log('C is fun');
});
$ guillaume@ubuntu:~/0x12$ ./101-main.js
C is fun
C is fun
C is fun
$ guillaume@ubuntu:~/0x12$ 
```

### 16. Add me maybe
Write a function that increments and calls a function.

* The function must be visible from outside
* Prototype: `function (number, theFunction)`
* You are not allowed to use `var`

**Solution:** [102-add_me_maybe.js](https://github.com/Emeralda0144/alx-higher_level_programming/blob/master/0x12-javascript-warm_up/102-add_me_maybe.js)

```
$ guillaume@ubuntu:~/0x12$ cat 102-main.js
#!/usr/bin/node
const addMeMaybe = require('./102-add_me_maybe').addMeMaybe;
addMeMaybe(4, function (nb) {
  console.log('New value: ' + nb);
});
$ guillaume@ubuntu:~/0x12$ ./102-main.js
New value: 5
$ guillaume@ubuntu:~/0x12$ 
```

### 17. Increment object
Update this script by adding a new function `incr` that increments the integer `value`.

* You are not allowed to use `var`

**Solution:** [103-object_fct.js](https://github.com/Emeralda0144/alx-higher_level_programming/blob/master/0x12-javascript-warm_up/103-object_fct.js)

```
$ guillaume@ubuntu:~/0x12$ cat 103-object_fct.js
#!/usr/bin/node
const myObject = {
  type: 'object',
  value: 12
};
console.log(myObject);
/*
YOUR CODE HERE
*/
myObject.incr();
console.log(myObject);
myObject.incr();
console.log(myObject);
myObject.incr();
console.log(myObject);

$ guillaume@ubuntu:~/0x12$ ./103-object_fct.js 
{ type: 'object', value: 12 }
{ type: 'object', value: 13, incr: [Function] }
{ type: 'object', value: 14, incr: [Function] }
{ type: 'object', value: 15, incr: [Function] }
$ guillaume@ubuntu:~/0x12$
```
