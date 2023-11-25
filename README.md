# jtsguide
`The guide is for learning and deep dive into JavaScript world!`

# Table of content
1. JavaScript: The language of internet
2. To be added later

# JavaScript: The language of internet
## Introduction to JS
The majority of modern websites uses JS, and all modern web browsers making it most ubiquitous programming language. In short, JS is high level, dynamic, untyped interpreted programming language that is suited to both object oriented and functional paradigm as well. JS was first used for scripting but, in recent decades it has evolved much more.

The name "JavaScript" is misleading. Except for a superficial syntactic resemblence, JavaScript is completely different from Java programming language. And JavaScript has since long outgrown its scripting language to become a robust and efficient programming language. The latest version of language defines new features for serious large scale software development.

The core JavaScript language defines minimal API for working with text, arrays, dates and regular expressions but does not include any input or output functionality. Input and output (and more features like storage, networking, graphics) are the responsibility of host environment in which JavaScript is embedded.

## Core JS
### Lexical structure
The lexical structure is a set of elementary rules specifying construct of programming language. It is lowest level syntax of a language. It specifies things like variable naming, delimiter characters, comments, statements and etc.

#### Character Set
JavaScript is written using Unicode character set. Unicode is superset of ASCII and Latin-1 and supports virtually every written language.

- Case sensitivity
  - JavaScript is case sensitive language i.e "Apple" and "apple" are two different interpreted literals.
  - Keywords, variables, function names and other identifiers should be written consistently.
- Comments
  - JavaScript supports two styles of comments i.e. Single line comment and Multiline comment.
  - Single Line comment starts with // and all the text followed in the line is ignored by interpreter.
  - Any text between /* and */ is treated as multiline comment.
- Identifiers and Reserved words
  - JavaScript identifiers must begin with a letter, digits, underscore or a dollar sign($) followed by letters, digits, underscore or dollar signs.
  - Digits are not allowed as first character so that JavaScript can easily distinguish between identifiers and numbers.
  - Reserved words are as follows
    - break, delete, function, return, typeof, case, do, while, if , switch, var, catch, else, in, this, void,  continue, false, instanceof, throw, debugger, finally, new, true, with, default, for, null, try, class, const, enum, export, extends, import, super and more
  - Global variables and functions are as follows
    - arguments, Array, Boolean, Date, decodeURI, decodeURIComponent, encodeURI, encodeURIComponent, Error, eval, EvalError, Function, Infinity, isFinite, isNaN, JSON, Math, NaN, Number, Object, parseFloat, parseInt, RangeError, ReferenceError, RegExp, String, SyntaxError, TypeError, undefined, URIError
- Optional Semicolons;
  - JavaScript uses semicolons(;) to separate statements. But, you can omit the use of semicolon if the statements are written on separate lines.
  - You can omit the semicolon at the end of program or if the next token in the program is a closing brace(})


### Types, Value and Variables
The types supported by JavaScript can be majorly divided into two categories.
1. Primitive types (e.g. numbers, strings, booleans)
2. Object types

And, there are few special primitive types like `null` and `undefined`. Any value that is not in primitive type is object type. An object is collection of properties having values associated. Well, function is also an object. In JavaScript terms, function is an object which has executable code inside it. Classes are also objects.

JavaScript interpreter performs automatic garbage collection for memory management. Programs can create objects as needed and never worry about dellocation of objects. When an object is no longer reachable, interpreter will automatically reclaim the memory so that it could be used for other tasks.

Let's dive deep into each type individually

1. Numbers
  JavaScript does not distinguish between integer values and floating point values. **All numbers are represented as floating point values** using 64-bits.
  - Integer literals
    Integers are written as a base 10 values. Hexadecimal values begins with "0x" or "0X" followed by string of hexadecimal value.
  - Floating point literals
    Floating point literals have decimal point. A real value is represented as the integral part of number, followed by decimal point and the fractional part of the number. They can also be represented using exponential notation: a real number followed by the letter e or E, followed by an optional plus or negative sign followed by an integer exponent. The notation represent the real number multiplied by 10 to power of the exponent.

**Few things to note**
Arithematic in JavaScript does not raise errors in case of overflow, underflow or division by zero. When the result of a numeric operation is larger than the largest representable number(overflow), the result is a special infinity value i.e. `Infinity`. On other hand, when a negative value becomes larger than the largest representable value, the result is a special negative infinity i.e. `-Infinity`.

If underflow occurs due to negative value, a special value is returned `negative zero`. On other hand, if underflow occure due to positive value, only `zero` is returned. `negative zero` is completely indistinguishable from `zero` and programmers rarely need to detect it.

Division by zero is not an error. It simply returns infinity or negative infinity. But, there is one exception, if zero is divided by zero does not have a well defined value, and the result is the special value i.e `NaN`. `NaN` also results because of division of inifinity by infinity or take square root of negative number or use of arithematic operators with non-numeric operands that cannot be converted to numbers. `NaN` has one speciality that it do not compare to other values except itself. That means, we cannot compare x to NaN. Instead, you should write `x!=x`, expression will be true only x is NaN.

2. Date and Times
   Core JavaScript include a Date() constructor for creating objects that represent dates and times. The object have methods provided for simple date calculations. Following are the methods commonly used for dates
   1. getFullYear()
   2. getMonth() //zero based
   3. getDate() // 1 based
   4. getDay() // 0 is sunday
   5. getHours() 
   6. getUTCHours()
   7. toString()
   8. toUTCString()
   9. toLocaleDateString()
   10. toLocalTimeString()
   11. toISOString()



### Expressions and Operators

### Statements

### Objects

### Arrays

### Functions

### Classes and Modules

### Regular expressions

### And more