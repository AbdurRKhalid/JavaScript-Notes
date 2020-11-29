This file contains the notes from the **Getting into JavaScript** at the **FrontendMasters** by the **Getify**.

### Overloaded Operators

The operators in programming world that can perform multiple tasks. For example, **+** can be used for the addition as well as concatinating the strings as well.

    var sum = 5 + 10;
    var combinedString = "This is a Dog " + "and his name is Zoroo.";

### Uniary Operators

Operators that only needs one operand to be applied on.

    !true //Here the '!' is a Uniary operator.

### Binary Operators

The Operators that Requires the Two Operators to Be Applied on.

    var age_days = age * 365; //Here '*' is the Binary Operator.

### Interpolated String

The string that contains the variables is called the Interpolated String.

    console.log(`This is an interpolated ${string}.`);

## Three Main Pillers of JavaScript

The following three concepts are the main pillers of the JavaScript and they are very important to know and to work in JavaScript as well.

1. Types/Coercion.
2. Scope/Closures.
3. this/Prototypes.

### Types

There are following types exists in the JavaScript:

- Primitive Types.
- Converting Types.
- Checking Types.

#### Primitive Types

- Undefined
- number
- string
- boolean
- object
- symbol
- **null (not Primitive but behaves like)**
- **function (subtype of object)**
- **Array(subtype of object)**
  _In JavaScript the variables does not have types but values have types._

### NaN

- Represents _"Not a Number"_.
- Occurred when mathamatical operation is
  performed on a non-mathamatical operands.

### new

- Used to created the new instances.
- Starts with capital letter.

The following does not require a _new_ keyword:

1. String()
2. Number()
3. Boolean()

## Coercion

The action of implicitly or explicitly converting one data type into other data type is called coercion in the JavaScript.

| Falsy                                                                         | Truthy                                                                |
| ----------------------------------------------------------------------------- | --------------------------------------------------------------------- |
| Values that Will become **false** when we will convert them into the booleans | Values that Will Become **true** when we will them intot the booleans |
| "", 0,-0, null, NaN, false, Undefined                                         | Everything Other Than Falsy is Truthy                                 |

## Equality

**==** vs **===**

1. _==_ is applied when the Coercion is Different.
2. _===_ is applied when the Coercion is Same.

**_When We know the Type then We Should Apply == instead of ===_**

### Function Expression

The function assigned to other variable is called the Function Expression.

    var sum = function add(num1, num2){
        return num1 + num2;
    }

### IIFE

- Immediately Invoked Function Expression.
- Functions that are declared
  and used at the same time.

(function printMessage() {
console.log("Hello World!");
} () )

### let

The _let_ keywords allows the following things:

- Allows the Encapsulation.
- Allows the Block Scoping.
- We cannot accessthe _let_ variables outside the block.

## Closure

Closure occurs when a function remembers the variables outside of the it, even if you pass that function somewhere else.
**_"Functions are First Class Variables!"_**

    function ask(question){
    	setTimeout(function waitASec() {
    		console.log(question);
    	}, 500)
    }

Now in the above function, the waitASec() function will be get called after 500ms so the question variable is remembed by the function.

## Prototypes

**Have to Read About it Still.**

## this

this keyword describes the usage of variable of value with respect to the context in which the variable is being used.

    function ask(question){
        console.log(this.teacher, question);
    }
    function otherClass(){
        var context = {
    	    teacher: 'James'
        };
        ask.call(context, 'What is Programming!');
    }

Here as we can see that ask() method is not receiving any parameter named teacher, but in context we can access that.
