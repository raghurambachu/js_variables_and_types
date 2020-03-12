# Value, Variables and Types

To understand store of value we need to understand value first. What is value? How do we store them?

# 1. What is Value

The most fundamental unit of information in programming is called value or data. It can be any piece of information like your name or age.

For example

`name` can be `"Arya"` or `age` can be `23`.

`"Arya"` and `23` in programming terms are called values.

You can have different kind of values a letter, word, paragraph, number etc. These values are divided into different types also know `Data Types` or you can call it value types. All the value has to be one of the following types.

## Data Types

1. Number (`21`, `21.45` )
2. String (`"a"`, `"hello"`, `"A quick brown fox jumped over lazy dog!"`)
3. Boolean (`true`, `false`)
4. `null`
5. `undefined`
6. Object

Latest addition to JavaScript family:

7. **Symbol**
8. **BigInt**

### Number

All numeric values are of `number` data type in JavaScript. Example of number type would be

    133, 1, 456 // Integers
    -123 , -324 // Negative Numbers
    132.43, -12.23 // Decimal point number
    Infinity, NaN, -Infinity // Special numbers like

**JavaScript uses a fixer number of bits i.e `64` to store a single number.**

Special numbers are values that are of number data type but doesn't exactly behaves like numbers in some cases.

    Infinity - 1 // Infinity

---

### BigInt

Used to represent the number bigger than 9007199254740991 or smaller than -9007199254740991. For BigInt you need to add `n` at the end of the value.

    const bigInt = 1234567890123456789012345678901234567890n;

---

### String

Any representation of text is `string` data type in JavaScript.

Example:

    "a" // letter
    "A" // uppercase letter
    "Hello" // word
    'Hello World!' // single quote
    "JavaScript is a single threaded language!" // paragraph

**Visual Impression to identify string:** Anything wrapped in `''` , `""` or `backticks` is a string.

---

### Boolean

To differentiate between only two possible values like `day` or `night` , `yes` or `no` , `on` or `off` we use boolean data type in JavaScript that has only two fixed values `true` or `false`.

`true` can represent values like `on` or `yes`

`false` represents values like `off` or `no`

---

### Void Values (Empty)

To represent the existence of no meaningful values we use special values i.e `null` or `undefined`. These are values that carry no informations. It is used for the places where the operation doesn't produce meaningful value.

`undefined` is the only value of type undefined `null` is the only value of type null

There is no fundamental difference between `null` or `undefined`. In most of the case you can treat the as interchangeable.

---

## `typeof`

To check the data type of any value we use `typeof` operator. It always return `string` data types.

    typeof 21; // "number"
    typeof "Hello"; // "string"
    typeof true; // "boolean"
    typeof undefined; // "undefined"
    typeof null; // "object" 🔥Boop

`typeof null` returns `"object"` is a bug in JavaScript. It can't be fixed ever because there are lots of website depends on this error.

## Predefined Utilities ( `alert`, `prompt`, `confirm`, `console`)

There are few predefined functions present in browser to help us interact with user and also to help us with debugging. These functions can be executed with `()` after the function name in browser using developer tool `console`

### `**alert**`

It accepts a message in string data type. This will open a dialog box in the browser with `ok` button.

The job of the alert function is to display a dialog box with any message you pass in the browser.

    alert('Hello World!');

### `prompt`

It accepts a string data type and display with an input box where user can enter value in the browser. `prompt` returns the data entered by user in the string data type.

    propmt("What is your age?"); // "21"

### `confirm`

It shows a modal window in the browser with two buttons i.e `ok` and `cancel` . It returns `true` if your click `ok` or `false` if you click `cancel`

    confirm("Do you want to close is?"); // true

- Type Conversion
  - Implicit
  - Explicit
- Operators
  - Logical (`&&` , `||`, `!`)
  - Comparison (`==`, `===`)
  - Conditional Operator
- Conditions
  - `if else`
  - `switch`
- Loops
  - `while`
  - `for`
