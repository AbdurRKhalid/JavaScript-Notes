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

1. Types/Coercin.
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
