#Lesson two.

Java utilizes specific primitive data types for basic values, along with the non-primitive `String` type. Variables must be declared with a type, can be initialized with a value, and their values can be reassigned during the program's execution.
##Primitive Data Types and String:
Primitive data types are the basic building blocks of data manipulation in Java, storing the value directly in memory. 
`int`: Stores integer (whole) numbers without decimals, such as 123 or -45. It is a 32-bit signed integer type.
`double`: Stores floating-point (decimal) numbers, such as 19.99 or -12.5. It offers double precision and is the default for decimals.
`boolean`: Stores logical values with only two possible states: true or false. It is primarily used in conditional statements.
`char`: Stores a single 16-bit Unicode character, such as 'a' or 'B'. Character values must be enclosed in single quotes.
`String`: This is a non-primitive, reference data type (a class) that stores a sequence of characters, such as `"Hello World"`. String values must be enclosed in double quotes.
Variable Declaration, Initialization, and Assignment 

Declaration is the process of defining a variable's type and name, essentially reserving a storage spot in memory. 
java
`int score; // Declares an integer variable named 'score' 
double price; // Declares a double variable named 'price' 
String name; // Declares a String variable named 'name' 
Use code with caution.`
`Initialization is assigning an initial value to a variable, which can be done at the time of declaration or later. Java requires variables to have a value before they can be used.
int lives = 3; // Declaration and initialization in one line
boolean isGameOver = false; // Declaration and initialization
Use code with caution.`

Assignment is changing the value of a variable that has already been declared. This can be done as many times as needed. 
java
`int x = 7; // Initialization
x = 12; // Assignment (changing the value of x to 12)
price = 9.99; // Assignment to a previously declared variable
name = "Java"; // Assignment to a previously declared String
Use code with caution.`

Basic Arithmetic Operations
Java supports standard arithmetic operators for numeric types. The result of an operation between two integers will be an integer; to get a decimal result, at least one operand should be a double. 
Operator 	Name	  Description
`+`   	Addition	Adds two values.
`-`	  Subtraction	Subtracts one value from another.
`*`	 Multiplication	Multiplies two values.
`/`	 Division	Divides one value by another.
`%`	 Modulus	Returns the division remainder.

Here is a demonstration of basic arithmetic operations:
java
        `public class ArithmeticDemo { 
            public static void main(String[] args) {
                int a = 10;
                int b = 3;
            // Integer operations
            int sum = a + b;         // 10 + 3 = 13
            int difference = a - b;  // 10 - 3 = 7
            int product = a * b;     // 10 * 3 = 30
            int quotientInt = a / b; // 10 / 3 = 3 (integer division truncates the decimal)
            int remainder = a % b;   // 10 % 3 = 1 (the remainder of 10 divided by 3)
            System.out.println("Integer Sum: " + sum);
            System.out.println("Integer Difference: " + difference);
            System.out.println("Integer Product: " + product);        System.out.println("Integer Quotient: " + quotientInt);
            System.out.println("Integer Remainder: " + remainder);
            // Double operations
            double x = 10.0;
            double y = 3.0;
            double quotientDouble = x / y; // 10.0 / 3.0 = 3.333...
            // Performing division with an int and a double results in a double
            double mixedQuotient = a / y; // 10 / 3.0 = 3.333...
            System.out.println("Double Quotient: " + quotientDouble);
            System.out.println("Mixed Type Quotient: " + mixedQuotient);
        }
     }`
