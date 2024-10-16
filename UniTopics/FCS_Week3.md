# Foundations of Computer Science Week 3

# Arithmetics in Java
- ## Arithmetic operations
  - *--> multiplication operator
  - Like in math, multiplcation and division take priority over addition and subtraction
  - We can use round brackets to force the order of operations
  - With 2 integer operands, the division returns an integer quotient, discarding remainder
  - The module operator returns the remainder of the division between integers
- ## Rounding
  -  The forced conversion [type cast](FCS_Week2.md) truncates the fractional part
  -  To carry out this conversion with rounding, preserving a more accurate value, we can use the Math.round() function
  -  Example :
    - Value = 2.75
    - Using type cast --> value = 2
    - Using Math.round() --> value = 3 
- ## Math functions
  - Math.pow(b, e) --> returns b^e
  - Math.sqrt(x) --> returns the square root of x
  - Math.log(x) --> returns the natural logarithm of x
  - Math.sin(x) --> returns the sine of x in radians
# Static Methods
  - class names (Math, System) start with a capital letter
  - object (out) and method (println, round) names start with a lowercase letter 
- ## Signature
- __**public static long round (double a)**__
  - public --> The method can be called in any other class
  - static --> the method is static (non static methods exist)
  - long --> type of data returned by the method
  - round --> name of the method (identifier)
  - (double a) --> explicit argument of the method
- ## Calling a static method
  -  values are passed through the arguments
    - int intRate = (int)Math.round(rate)
  - Syntax : _ClassName.methodName(arguments)_ 
# Complements of Java Syntax
- ## Combining assignment and arithmetic statements
  - ```java
    x = x + 2 --> x += 2
    x = x*2 --> x *= 2
    ```
- ## Variable increment/decrement
  - ```java
    x = x + 1 --> x++
    x = x - 1 --> x--
    ```
- ## Variables without init / missing init of variables
  - Variables can created without initialization
  - In this case, the space for the varieble gets reserved in memory, but it isnt empty, it contains a random value
  - If we use this variable without effectively initializing it, the compiler returns a compile time error
- # Strings
  - ## The String Data Type
    - While numbers are primitive data types, Strings are objects, which means they can call methods contained in the String class
    - Counting Characters :
      - length() method
      - not static
      - ```java
        String s = "aaa"
        s.length()
        ```
    - Extraction of a substring :
    - substring(beginIndex, endIndex)
    - returns a string based on the start and end index given
    - we can also jut put beginIndex in the arguments, and the method returns the substring from the index indicated to the end of the original string 
    - ```java
      String s = "abcd"
      Indexes --> 0123
      s.substring(0, 3) --> returns abc
      s.substring(1) --> returns bcd
      ```
    - String concatenation :
      - To concatenate strings we use the **+** operator
      - Any item concatenated turns into a string
      - No space added between items
 -  ## Useful Methods - String class
   - toUpperCase() : converts the whole string to upper case
   - toLowerCase() : converts the whole string to lower case
# Escape Sequences
 - the backslash character is used to insert escxape sequences into the code
 - to insert the backslash character into a string, for example, we use the double backslash (\\)
 - \n --> newline
 - We can also use the \ character to insert foreign characters
 - ```java
   System.out.println("Frapp\u00E9?"); --> Frappè?
   ```
# Char Primitive Data Type
# Introduction to Classes and Objects
 - ## Motivations
 - ## Objects
 - ## Classes
 - ## Using a class
 - ## Calling instance methods
 - ## Overloaded names of methods
 - ## Creating and instancing objects
 - ## Classes - Public interface 
 - ## Creating and using objects
 - ## Accessor and mutators instance methods
 - ## Constructor of the java.lang.String class

# Acquiring data from the user
- ## Motivations
- ## Acquiring data from the user
- ## Acquiring data from an input dialog box
- ## Presenting data to operators by message dialog box
- ## Acquiring data from standard input
 - All Java programs have acces to their Standard output through the System.out object.
 - Similarly, the System.in object makes the input stream available to running programs
 - The Inputstream class makes the read() method available to read one byte at a time
- ## Using the java.util.Scanner class
 - From JDK 5, the Scanner class was introduced, and it provides a convenient interface to the System.in object
 -  Lets define a new Scanner object
 -  ```java
    Scanner in = new Scanner(System.in);
    ```
 - The constructor argument is a reference to a java.io.InputStream class object
 - System.in is an instance of the java.io.InputStream class
 - Scanner defines eight constructors
 - Now that ew have defines a Scanner object, lets acquire data from Standard input
 - ```java
   Scanner in = new Scanner(System.in);
   System.out.print(“Enter an integer ”);
   int n = in.nextInt();
   System.out.println(“Entered: “ + n);
   ```
 - The nextInt() method waits for data to be entered
 - By using the double nextDouble() method, we can acquire floating point numbers
 - To acquire a word, i.e. a string delimited by chars SP, '\ t', '\ n', '\ r'): String next() method
 - ```java
   System.out.print(“Enter a word: ”);
   String s = in.next();
   System.out.println(“Word entered: “ + s);
   ```
 - To acquire a line, i.e. a string delimited by the chars '\ n' or '\ r'): String nextLine ()
method
 - ```java
   System.out.print(“Enter one or more words: ”);
   String s = in.nextLine();
   System.out.println(“Line entered: “ + s);
   ```
 - *__Since the Scanner class is not part of the java.lang package, but of the java.util
package, it is necessary to import the class before using it__*
 - Its advisable to close the Scanner class object once we're done with it
 - ```java
   in.close_();
   ```

# Java packages
- ## Syntax - Importing classes from packages
- ## Styles for importing classes

# Converting strings to numbers and numbers to strings
- ## How to convert strings into numbers 
- ## Converting a string into a floating point number 
- ## Converting numbers into strings
# Number Formatting


# Compile time errors
# Runtime errors





















