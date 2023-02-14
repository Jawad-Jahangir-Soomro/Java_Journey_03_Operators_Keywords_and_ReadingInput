
# Java Journey, 03: Operators, Keywords, and Reading Input

The 03 repository covers the concept of operators and keywords in Java, along with their usage. It also delves into reading input from the user and using it in the program. By mastering this repository, you'll be able to create programs that can take user input and perform a variety of operations on that data using different operators and keywords.

## Learn about the different operators available in Java.

In Java, operators are symbols that perform operations on one or more operands, which can be variables, literals, method returns, or expressions. 
There are different types of operators available in Java, including:

### 1 - Arithmetic Operators: 

Arithmetic operators are used to perform basic arithmetic operations like addition, subtraction, multiplication, division, and modulus on numeric data types in Java.

The following are the arithmetic operators available in Java:

- Addition (+): adds two values and returns their sum. For example, int result = 5 + 2; would assign the value 7 to the variable result.

- Subtraction (-): subtracts one value from another and returns the result. For example, int result = 5 - 2; would assign the value 3 to the variable result.

- Multiplication (*): multiplies two values and returns their product. For example, int result = 5 * 2; would assign the value 10 to the variable result.

- Division (/): divides one value by another and returns the quotient as a double value. For example, double result = 5.0 / 2.0; would assign the value 2.5 to the variable result.

- Modulus (%): returns the remainder of dividing one value by another. For example, int result = 5 % 2; would assign the value 1 to the variable result.

It's important to note that when using arithmetic operators, the data types of the operands must match. 

For example, you cannot add an int and a double without first casting one of the operands to the appropriate type.

Example:


```bash
    int num1 = 10;
    int num2 = 4;
    int sum = num1 + num2; // sum is 14
    int difference = num1 - num2; // difference is 6
    int product = num1 * num2; // product is 40
    double quotient = (double) num1 / num2; // quotient is 2.5
    int remainder = num1 % num2; // remainder is 2

```

### 2 - Assignment Operators:

In Java, assignment operators are used to assign values to variables. They are represented by various symbols such as "=" (simple assignment operator), "+=" (additive assignment operator), "-=" (subtraction assignment operator), "*=" (multiplication assignment operator), "/=" (division assignment operator), "%=" (modulus assignment operator), "&=" (bitwise AND assignment operator), "|=" (bitwise OR assignment operator), "^=" (bitwise XOR assignment operator), "<<=" (left shift assignment operator), ">>=" (signed right shift assignment operator), and ">>>=" (unsigned right shift assignment operator).

The basic format of an assignment operator is:

variable operator= expression;

Here, "variable" represents the variable that is being assigned a value, "operator" represents the assignment operator, and "expression" represents the value that is being assigned to the variable.

For example, the statement "x += y" is equivalent to "x = x + y". Similarly, the statement "x *= y" is equivalent to "x = x * y".

Example:

```bash
int x = 10;
int y = 5;

x += y; // equivalent to x = x + y
System.out.println(x); // Output: 15

x -= y; // equivalent to x = x - y
System.out.println(x); // Output: 10

x *= y; // equivalent to x = x * y
System.out.println(x); // Output: 50

x /= y; // equivalent to x = x / y
System.out.println(x); // Output: 10

x %= y; // equivalent to x = x % y
System.out.println(x); // Output: 0

x &= y; // equivalent to x = x & y
System.out.println(x); // Output: 0

x |= y; // equivalent to x = x | y
System.out.println(x); // Output: 5

x ^= y; // equivalent to x = x ^ y
System.out.println(x); // Output: 0

x <<= y; // equivalent to x = x << y
System.out.println(x); // Output: 0

x >>= y; // equivalent to x = x >> y
System.out.println(x); // Output: 0

x >>>= y; // equivalent to x = x >>> y
System.out.println(x); // Output: 0

```

In the above example, the value of variable "x" is updated using different assignment operators. The output of the program shows the updated value of "x" after each assignment.

### 3 - Comparison Operators:

In Java, comparison operators are used to compare two values and return a boolean value (true or false) depending on whether the comparison is true or false. There are six comparison operators in Java, listed below:

- Equal to (==): Returns true if two values are equal, otherwise false.
- Not equal to (!=): Returns true if two values are not equal, otherwise false.
- Greater than (>): Returns true if the first value is greater than the second value, otherwise false.
- Greater than or equal to (>=): Returns true if the first value is greater than or equal to the second value, otherwise false.
- Less than (<): Returns true if the first value is less than the second value, otherwise false.
- Less than or equal to (<=): Returns true if the first value is less than or equal to the second value, otherwise false.

Here are some examples of how comparison operators work in Java:

```bash
    int x = 5;
    int y = 7;

    boolean result = (x == y); // false
    result = (x != y); // true
    result = (x > y); // false
    result = (x >= y); // false
    result = (x < y); // true
    result = (x <= y); // true

```

In the above example, we initialize two integer variables x and y. We then use comparison operators to compare the values of x and y, and assign the result to a boolean variable called result. Depending on the values of x and y, the result will be either true or false.

### 4 - Logical Operators:

Logical operators are used to evaluate two or more conditions in a boolean expression. There are three logical operators in Java: && (logical AND), || (logical OR), and ! (logical NOT).

- The && operator returns true if both conditions on either side are true.

    Example:

    ```bash
    int x = 5, y = 10;

    if (x > 3 && y < 15) {
        System.out.println("Both conditions are true");
    }

    ```

- The || operator returns true if either one of the conditions on either side is true.

    Example:

    ```bash
    int x = 5, y = 10;

    if (x > 3 || y > 15) {
        System.out.println("At least one condition is true");
    }

    ```

- The ! operator negates the value of a boolean expression. If the expression is true, the operator returns false; if the expression is false, the operator returns true.

    Example:

    ```bash
    boolean a = true, b = false;

    if (!a) {
        System.out.println("a is false");
    }
    if (!b) {
        System.out.println("b is true");
    }

    ```

### 5 - Bitwise Operators:

In Java, bitwise operators are used to perform operations on individual bits of a binary number. They work with integers at the bit level and are applied to each pair of corresponding bits of the two operands. Here are the bitwise operators in Java:

- AND (&): This operator sets each bit to 1 if both bits are 1.

    Example:

    ```bash
    int a = 5 & 3;

    // binary representation: 101 & 011
    // result: 001 (which is 1 in decimal)

    ```

- OR (|): This operator sets each bit to 1 if either bit is 1.

    Example:

    ```bash
    int a = 5 | 3;

    // binary representation: 101 | 011
    // result: 111 (which is 7 in decimal)

    ```

- XOR (^): This operator sets each bit to 1 if only one of the two bits is 1.

    Example:

    ```bash
    int a = 5 ^ 3;

    // binary representation: 101 ^ 011
    // result: 110 (which is 6 in decimal)

    ```

- NOT (~): This operator inverts all the bits of an integer, turning 0 into 1 and 1 into 0.

    Example:

    ```bash
    int a = ~5;
    
    // binary representation: ~101
    // result: 11111111111111111111111111111010 (which is -6 in decimal)

    ```

- Left shift (<<): This operator shifts the bits of an integer to the left by a specified number of positions. The leftmost bits are discarded and zeros are added to the right.

    Example:

    ```bash
    int a = 5 << 2;

    // binary representation of 5: 101
    // binary representation of 20: 10100
    // result: 20

    ```

- Right shift (>>): This operator shifts the bits of an integer to the right by a specified number of positions. The rightmost bits are discarded and zeros are added to the left.

    Example:

    ```bash
    int a = 20 >> 2;

    // binary representation of 20: 10100
    // binary representation of 5: 101
    // result: 5


    ```

- Unsigned right shift (>>>): This operator is similar to the right shift operator, but it fills the leftmost bits with zeros instead of the sign bit. This is useful for shifting unsigned values.

    Example:

    ```bash
    int a = -20 >>> 2;

    // binary representation of -20: 11111111111111111111111111101100
    // binary representation of 1073741823: 00111111111111111111111111111111
    // result: 1073741823



    ```

### 6 - Ternary Operator:

In Java, a ternary operator is a shorthand for an if-else statement. It consists of three operands and is denoted by the ? : symbol. It can be used to write concise code and is commonly used in control flow statements.

The syntax for a ternary operator is as follows:

```bash
variable = (condition) ? value1 : value2;
```

If the condition is true, then the value of the expression is value1, otherwise it is value2.

Here's an example:

```bash
int num1 = 5;
int num2 = 10;
int maxNum = (num1 > num2) ? num1 : num2;
```

In this example, the ternary operator is used to assign the value of the variable maxNum. If num1 is greater than num2, then maxNum will be assigned the value of num1. Otherwise, maxNum will be assigned the value of num2.

Another example of a ternary operator:

```bash
int x = 10;
String result = (x > 5) ? "x is greater than 5" : "x is less than or equal to 5";
```

In this example, the ternary operator is used to assign the value of the variable result. If x is greater than 5, then result will be assigned the string "x is greater than 5". Otherwise, result will be assigned the string "x is less than or equal to 5".


## Study the use of keywords in Java.

keywords are reserved words that have predefined meanings in the programming language. These words cannot be used as identifiers such as variable names or method names. Understanding the usage of keywords is important as it allows developers to write correct and efficient code.

Java has 57 keywords, which are Categorized as: 

- Access modifiers: public, private, protected.

- Control flow statements: if, else, switch, case, default, while, do, for, break, continue, return.

- Data types: byte, short, int, long, float, double, char, boolean, void.

- Class-related keywords: class, interface, enum, extends, implements, super, this, new, instanceof.

- Exception handling: try, catch, finally, throw, throws.

- Modifiers: abstract, final, static, synchronized, native, transient, volatile.

- Object-related: true, false, null.

- Miscellaneous: assert, enum, package, import.

These keywords have specific meanings in the Java programming language, and using them incorrectly or improperly can lead to syntax errors.

Here are a few things to keep in mind when studying the use of keywords in Java:

- Keywords cannot be used as variable names, method names, or class names.

- Keywords are case sensitive and must be written in lowercase letters.

- It is important to be familiar with the different keywords and their meanings in order to write correct and efficient code.

For example, the "public" keyword in Java is used to specify that a class or method can be accessed from anywhere in the program. The "static" keyword is used to indicate that a method or variable is associated with a class rather than an instance of a class. Understanding the meanings and appropriate usage of these keywords is crucial for writing effective Java code.

### Access Modifiers

In Java, access modifiers are used to restrict the visibility or accessibility of classes, methods, and variables. There are four types of access modifiers in Java:

- Public: A public class, method, or variable can be accessed from anywhere in the program.

    Example

    ```bash
    public class Example {
        public void display() {
            System.out.println("This is a public method");
        }
    }
    ```

- Private: A private class, method, or variable can only be accessed within the same class.

    Example

    ```bash
    public class Example {
       private String name;
   
        public void setName(String name) {
            this.name = name;
        }
    }

    ```

- Protected: A protected class, method, or variable can be accessed within the same class, subclasses, and classes in the same package.

    Example

    ```bash
    public class Animal {
        protected String name;
   
        protected void eat() {
            System.out.println("The animal is eating.");
        }
    }

    public class Dog extends Animal {
        public void bark() {
            System.out.println("The dog is barking.");
        }
    }
    
    ```


- Default: A class, method, or variable with no access modifier specified can only be accessed within the same package.

    Example

    ```bash
    class Example {
    int num;
    
        void display() {
            System.out.println("The number is: " + num);
        }
    }

    
    ```

By using access modifiers, we can control the visibility of classes, methods, and variables in our Java programs, which helps to improve code readability and maintainability.

### Some other Keywords.

- <b>this</b> : 

    The this keyword refers to the current object in a method or constructor. The most common use of the this keyword is to eliminate the confusion between class attributes and parameters with the same name (because a class attribute is shadowed by a method or constructor parameter)

- <b>new</b> :

    The new keyword in Java instantiates a class by allocating desired memory for an associated new object. It then returns a reference to that memory. Many times, the new keyword in Java is also used to create the array object. The new keyword is followed by a call to a constructor, which instantiates the new object.

- <b>static</b> :

    The static keyword is a non-access modifier used for methods and attributes. Static methods/attributes can be accessed without creating an object of a class.

- <b>import</b> : 

    import is a Java keyword. It declares a Java class to use in the code below the import statement. Once a Java class is declared, then the class name can be used in the code without specifying the package the class belongs to. Use the '*' character to declare all the classes belonging to the package.
