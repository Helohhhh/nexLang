# Syntax Rules for NexLang  Language
## Syntax:
- To print stuff to the terminal
    - Syntax: `print("")` for printing stuff, and `print()` for printing raw data.
    - Example: 
      ```python
      print("Hello, World!")
      print(42)
      ```

- Naming variables:
    - Use "int" for naming variables that are integers.
    - Use "str" for naming variables whose value is a string.
    - Use "boo" for boolean variables.
    - Use "dict" for naming dictionary variables.
    - Use "list" for naming array variables.
    - Use "float" for naming floating-point variables.
    - Use "void" if the variable is undefined.
    
    Example:
    ```c++
    int value = 12
    let str name = "Alice"
    const boo isTrue = true
    dict person = {"name": "Bob", "age": 30}
    list numbers = [1, 2, 3]
    float pi = 3.14159
    void undefinedVar
    ```

- Variable Prefixes:
    - Prefix variable names with "let" for changeable variables and "const" for variables that cannot be changed.
    
    Example:
    ```python
    let int count = 5
    const str greeting = "Hello"
    ```

- Comments:
    - Use "//" or "#" for single-line comments.
    - Use "%" to start and end double-line comments for longer comments.
    
    Example:
    ```ruby
    // This is a single-line comment
    # Another single-line comment
    % This is a block-level comment %
    ```

- Loops and Conditionals:
    - Use "for i of times(_startingNum_, _endingNum_)" for loops that run a specific number of times.
    - Use "while this is True:" for creating an infinite loop.
    
    Examples:
    ```python
    for i of times(1, 5):
        // Loop from 1 to 5
    
    while this is True:
        // Infinite loop
    ```

- String Interpolation:
    - Use curly braces `{}` to interpolate variables and expressions within strings.
    
    Example:
    ```python
    str name = "Alice"
    console.print("Hello, {name}!")
    ```


- Destructuring Assignment:
    - Use destructuring assignment to extract values from arrays and objects.
    
    Example:
    ```python
    let [a, b] = [1, 2]
    let {name, age} = {name: "Bob", age: 30}
    ```

- Enums:
    - Define enumerations to represent named values.
    
    Example:
    ```python
    enum Color {
        RED,
        GREEN,
        BLUE
    }
    Color chosenColor = Color.GREEN
    ```

- Object-Oriented Programming:
    - Define classes and objects using the "class" keyword.
    
    Example:
    ```python
    class Person:
        str name
        int age
    
        func constructor(name, age):
            this.name = name
            this.age = age
    
    let person = new Person("Bob", 25)
    ```



- Concurrency and Asynchronous Programming:
    - Use "async," "await," and "promise" for asynchronous programming.
    
    Example:
    ```javascript
    async func fetchData():
        let data = await fetchDataFromAPI()
        console.print(data)
    
    fetchData()
    ```
- Miscellaneous Syntax ideas that i didnt think of before:
    - Ternary Operator: Use "$$" for a ternary operator.
    example: 
    ```javascript
    const int isEven = number / 2 === 0 $$ "The number is even" : "The number is odd"
    ```
    - String Methods:
        - str.length(): Returns the length(number of character including whitespaces) of the string
        Example:
        ```javascript
        let str data = "Text"
        const int length = data.length()
        ```
        - str.concat(other): Concatenates the current string with another string and returns the result.
        Example:
        ```javascript
        const str str1 = "Hello "
        const str str2 = "World!"
        const str result = str.concat(str2)
        ```
        - str.toUpperCase(): Converts all characters in the string to uppercase
        Example: 
        ```javascript
        const str data = "Hello World"
        const str result = data.toUpperCase()
        ```
        - str.toLowerCase():  Converts all characters in the string to lowercase.
        Example:
        ```javascript
        const str data = "Hello World"
        const str result = data.toLowerCase()
        ```
         will add more later
    - Data type Parameters: Data Type parameters in functions for improverd clarity and improved flexibility (**Note that the data type of the parameter cannot be changed!**)
    Example:
    ```javascript
    func addNum(num1: int, num2: int){
        return num1 + num2
    }
    ```
    - Array Comprehensions:  array comprehensions for creating arrays in a concise and expressive way.
    Example:
    ```javascript
    const list squares = [x * x for i of times(1, 6)]
    ```
    - Pattern Matching: pattern matching for more expressive and concise conditional statements.
    Syntax: PTM {value}: ...break;;;
    Example:
    ```javascript
    PTM value:
        case 0:
            console.print("0")
        case 1:
            console.print("1")
        case 2:
            console.print("2")
        case 3:
            console.print("3")
    break;;;
    ```
    - Custom Operators: Developers can create custom operators that they can use for domain specific syntax.
    Syntax: @funcName... -> {name of your custom operator}
    ```javascript
    @addNums(num1: int, num2: int) -> int -> ^^{
        return num1 + num2
    }
    const int result = 34 ^^ 23 //Result should be 57
    ```
    
