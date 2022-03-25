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
