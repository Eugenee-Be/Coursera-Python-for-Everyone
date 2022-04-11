# Learning Log

The learning progress is documented in this file.

## [Unreleased]


## 📘 Chapter 1: Week 1/2/3 Very Basic Intro [25-03-2022]

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

## 📘 Chapter 2: Week 4 Variables and Expressions [25-03-2022]

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
## 📘 Chapter 3: Week 5 Conditional Statements [29-03-2022]

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


## 📘 Chapter 4: Week 6 Functions [10-04-2022]

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

## 📘 Chapter 5: Week 7 Loops and Iteration [11-04-2022]


### 🚅 Outlines

* 1️⃣ Repeated steps
    * Keyword: ``` while ```
    * Example:
           
           
            while n > 0 :
                print(n)
                n = n - 1
            print('Blastoff!')
            print(n)
            
    * Infinite Loop:
           
            
            n = 5
            while n > 0 :
                print('Lather')
                print('Rinse')
            print('Dry off!')
            
       Iteration variable: n
    * Breaking out of a Loop ```break```
            
            
            while True:
                line = input('> ')
                if line == 'done':
                    break
                print(line)
            print('Done!')
            
       Escape the loop instantly
    * Finish an Iteration with Continue ```continue```
            
            
            while True :
                line = input('> ')
                if line[0] == '#' :
                    continue
                if line == 'done' :
                    break
                pirnt(line)
            print('Done!')
            
* 2️⃣ Definite Loops ```for```
    * A simple Definite Loop Example:
             
             
             for i in [5, 4 , 3, 2, 1] :
                print(i)
             print('Blastoff!')
             
    * A simple Definite Loop with Strings:
                
                
                friends = ['Joseph', 'Glenn', 'Sally']
                for friend in friends :
                    print('Happy New Year:', friend)
                print('Done!')
                
                
    * Move ```i``` ahead
    * Contract: for i in members
* 3️⃣ Finding the Largest Value
            
            
            largest_so_far = -1
            print('Before', largest_so_far)
            for the_num in largest_so_far :
                if the_num > largest_so_far :
                    largest_so_far = the_num
            
            print('After', largest_so_far)
            
* 4️⃣ Counting in a Loop
            
           
            zork = 0
            print('Before', zork)
            for thing in [9, 41, 12, 3, 74, 15] :
                zork = zork + 1
                print(zork, thing)
            print('After', zork)
           
* 5️⃣ Summing in a Loop
            
            
            zork = 0
            print('Before', zork)
            for thing in [9, 41, 12, 3, 74, 15] :
                zork = zork + thing
                print(zork, thing)
            print('After', zork)
            
* 6️⃣ Finding the Average in a Loop
            
            
            count = 0
            sum = 0
            print('Before', zork)
            for value in [9, 41, 12, 3, 74, 15] :
                count = count + 1
                sum = sum + value
                print(count, sum, value)
            print('After', count, sum, sum / count)
            
* 7️⃣ Filtering in a Loop
            
            print('Before')
            for value in [9, 41, 12, 3, 74, 15] :
                if value > 20 :
                    print('Large number', value)
            print('After')
 * 8️⃣ Search Using a **Boolean Variable**
            
            found = False
            print('Before', found)
            for value in [9, 41, 12, 3, 74, 15] :
                if value == 3 :
                    found = True
                    break
                print(found, value)
            print('After', found)
 
 * 9️⃣ How to Find the Smallest Value
            
            smallest_so_far = None
            print('Before')
            for value in [9, 41, 12, 3, 74, 15] :
                if smallest is None :
                    smallest = value
                elif value < smallest :
                    print(smallest, value)
            
            print('After', smallest)
            
* 1️⃣0️⃣ "is" and "is not" Operators
    * is: implies is the same as
    * strong equiality


### ❓ Questions

N/A

### ❗ Quiz summary

N/A

### ⛵ Further Exploration

N/A
