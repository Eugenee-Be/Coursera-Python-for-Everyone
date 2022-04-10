# Learning Log

The learning progress is documented in this file.

## [Unreleased]


## 📘 Chapter 1: Project 1/2/3 Very Basic Intro [25-03-2022]

### 🚅 Outlines

* [Python for Everybody website](py4e.com)
* Background knowledge
* Hardware
* Reserved words
* ``` quit() ``` exit the python programme 

### ❔ Questions

N/A

### ❗ Quiz summary

N/A

### ⛵ Further Exploration

* Fundation of Computer Systems

## 📘 Chapter 2: Project 4 Variables and Expressions [25-03-2022]

How a programme uses the computer's memory to store, retrieve and calculate information.

### ❗ Quiz summary

* Converting from float to integer only passes the value before the floating point _regardless how much the value is after the floating point_.
    
    ```
    x = int(98.6)
    print(x)
    ```
    Result
    ```
    98
    ```
* ```print('Hello', name)``` leaves a **[SPACE]** after "Hello" automatically

### 🚅 Outlines

#### Expressions

Key: Varibale Operator Constant Function

* 1️⃣ Variables
  * start with a letter or _(underscore)
  * case sensitive
* 2️⃣ Assignment statements =
* 3️⃣ Numeric Expressions
  * Operators
    | Operator | Funciton  |
    |----------| ----------|
    |      **  |      Power|
    |      %   |  Remainder|
* 4️⃣ Order of evaluation - Operator Precedence
* 5️⃣ Types of variable
  * ```type( )``` tells the type
* 6️⃣ Type Conversions
  * ```float( )``` converts integer to float
  * Integer Division: produces a _floating point result_
  * String conversion
    
    ❎ Conversion wrong attempt
    ```
    stringValue = '123'
    type(stringValue)
    print(stringValue + 1) WRONG!
    ```
    ➰ Conversion...
    ```
    integerValue = int(stirngValue)
    type(integerValue)
    print (integerValue + 1) CORRECT!
    ```
    ❎ No digits in string variable
    ```
    nsv = 'hello bob'
    niv = int(nsv) WRONG!
    ```
 * 7️⃣ User Input
   * input( ) function
     ```
     name = input('Who are you?')
     print('Welcome', name)
     ```
     If I type...
     ```
     Eugene
     ```
     The output should be...
     ```
     Who are you?
     (I typed here) Eugene
     Welcome Eugene
     ```
 * 8️⃣ Documentation - Comments
  
      ```x = 1 # Everything after '#' is ignored ```
 
 * 9️⃣ Converting User Input
  
      ```
      # Convert elevator floors
      inp = input('Europe Floor?')
      usf = int(inp) + 1
      print('US floor', usf)
      ```
## 📘 Chapter 3: Project 5 Conditional Statements [29-03-2022]

### 🚅 Outlines

* if (statement):
  * Indent
  * elif (statement):
  * else:
* Avoid Traceback: avoiding mistakes - Insurance policy
    * try/except
     ```
     astr = 'Hello Bob'
     try:
        istr = int(astr)
     except:
        istr = -1
     print('First', istr)
     
     astr = '123'
     try:
        istr = int(astr)
     except:
        istr = -1
     print('Second', istr)
     ```
    * Insurance policy: alternate code to run when programme blows up
    * Entire programme in _'try'_ block, if it blows up, go to _'except'_ block and print -1.
    * Only put code you are unsure about
* Sample try/except
 ```
 rawstr = input('Enter a number:')
 try:
    ival = int(rawstr)
 except:
    ival = -1
 
 if ival > 0:
    print('Nice work')
 else:
    print('Not a number')
 ```


### ❔ Questions

N/A

### ❗ Quiz summary

* Logical operators
    | Operator | Funciton       | Equal Syntax|
    |----------| ---------------|-------------|
    |     and  | x > 1 and x < 2| 1 < x < 2   |
    |     or   | x < 1 or x > 2 | /           |
    |     not  |not(x > 1 and x < 2| / |

### ⛵ Further Exploration

* Fundation of Computer Systems
* Arduino prototyping


## 📘 Chapter 4: Project 6 Functions [10-04-2022]

### 🚅 Outlines

* 1️⃣ Stored steps
    * Fundamentals
    ```
    def funcname():
        print('Hello')
        print('Fun')
    
    Calling/Invoking:
    funcname()
    ```
* 2️⃣ Built-in Functions
    * max/min()
    ```
    big = max('Hello world')
    print(big)
    
    Output:
    w
    ```
    * float/int()
    * type()
* 3️⃣ Builidng Functions
    * def: define the funciton
    * After define it, Call/Invoke the function!
    * Arguments
    ```
    def greet(lang):
        if lang == 'en':
        ...
    greet('en')
    ```
    lang is just an alias
    * return
        stops the function, determine residual value
    * Multiple arguments
     ```
     def addtwo(a, b):
        added = a + b
        return added
     ```
 
### ❓ Questions

N/A

### ❗ Quiz summary

N/A

### ⛵ Further Exploration

N/A

