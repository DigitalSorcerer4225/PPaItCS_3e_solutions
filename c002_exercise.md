# Exercises
## Review Questions
### True/False

**F**   1. The best way to write a program is to immediately type in some code and
        then debug it until it works.

**T**   2. An algorithm can be written without using a programming language.

**F**   3. Programs no longer require modification after they are written and de­
        bugged.

**T**   4. Python identifiers must start with a letter or underscore.

**F**   5. Keywords make good variable names.

**T**   6. Expressions are built from literals, variables, and operators.

**T**   7. In Python, x = x + 1 is a legal statement.

**F**   8. Python does not allow the input of multiple values with a single statement.

**T**   9. A counted loop is designed to iterate a specific number of times.

**F**   10. In a flowchart, diamonds are used to show statement sequences, and rect­
        angles are used for decision points.

### Multiple Choice

**c**   1. Which of the following is not a step in the software development process?
            
            a) specification 
            b) testing/Debugging 
            c) fee setting 
            d) maintenance
            
**a**   2. What is the correct formula for converting Celsius to Fahrenheit?
            
            a) F = 9/5(C) + 32 
            b) F = 5/9(C) - 32 
            c) F = B^2 -4AC
            d) F = (212-32)/(100-0)
            
**d**   3. The process of describing exactly what a computer program will do to solve
        a problem is called
            
            a) design 
            b) implementation 
            c) programming 
            d) specification
            
**c**   4. Which of the following is not a legal identifier?
            
            a) spam 
            b) spAm 
            c) 2spam 
            d) spam4U
            
**b**   5. Which of the following are not used in expressions?
            
            a) variables 
            b) statements 
            c) operators 
            d) literals
            
**b**   6. Fragments of code that produce or calculate new data values are called
            
            a) identifiers
            b) expressions
            c) productive clauses
            d) assignment statements
            
**b**   7. Which of the following is not a part of the IPO pattern?
            
            a) input
            b) program
            c) process
            d) output
            
**d**   8. The template, for <variable> in range (<expr>) describes
            
            a) a general for loop
            b) an assignment statement
            c) a flowchart
            d) a counted loop
            
**a**   9.Which of the following is the most accurate model of assignment in Python?
            
            a) sticky-note
            b) variable-as-box
            c) simultaneous
            d) plastic-scale

**d**   10. In Python, getting user input is done with a special expression called
            
            a) for 
            b) read 
            c) simultaneous assignment 
            d) input

### Discussion
1. List and describe in your own words the six steps in the software develop­
ment process.

    
    There are six main steps in the creation of a software. The first step is
    to understand the problem. In this step, the programmer's goal is to think
    about what the problem is and what it asks for. The second step is to determine
    the specifications of the program. In this step, the programner's goal is to
    determine what the program will do. It also helps to determine
    what the inputs, outputs, and how they relate together. The third step is to
    make an algorithm based on step two using a natural language. The fourth step
    is to translate the algorithm into a programming language. The fifth step is
    to test and debug the program. In this step, the programmer's goal is to test
    for all the possbile ways that the program breaks and fix that. The sixth step is to
    maintain and update the program based on the end-users' needs.

2. Write out the chaos.py program (Section 1.6) and identify the parts of
the program as follows:

- Circle each identifier.
- Underline each expression.
- Put a comment at the end of each line indicating the type of statement
on that line (output, assignment, input, loop, etc.).

``Note:``
 
    An expression is a syntactic entity in a programming language that may be evaluated 
    to determine its value. It is a combination of one or more constants, variables, 
    functions, and operators that the programming language interprets and computes to 
    produce another value.


5. Explain the relationships among the concepts: definite loop, for loop, and
counted loop.


    Definite loops are loops that iterate a command or series of command a specific number of times.
    For loops are definite loops in Python. Counted loops is a for loop pattern
    where a loop is specifically chosen to run a specific number of times.

7. Show the output from the following fragments:

    for i in range (5):<br>
    print (i * i)
        
        ``python
        0
        1
        4
        9
        16
        ``
    b) for d in [3,1,4,1,5]:
        print (d, end=" ")
        
        ``python
        3 1 4 1 5
        ``
        
    c) for i in range(4) :
        print ("Hello")
        
        ``python
        Hello
        Hello
        Hello
        Hello
        ``
    d) for i in range ( 5) :
        print (i, 2 **i)
        
        ``python
        0 1
        1 2
        2 4
        3 8
        4 16
        ``
8. Why is it a good idea to first write out an algorithm in pseudocode rather
than jumping immediately to Python code?


    It's easier to create an algorithm without the technical mental overhead
    when writing an algorithm in a programming language.
    
9. The Python print function supports other keyword parameters besides
end. One of these other keyword parameters is sep. What do you think
the sep parameter does? Hint: sep is short for separator. Test your idea
either by trying it interactively or by consulting the Python documentation.


    The sep keyword is used for determining what the separator will be used
    when separating arguments in the print function
    
10. What do you think will happen if the following code is executed?
    
     print ("start")
     for i in range (O) :
         print ("Hello")
     print ("end")


     Look at the flowchart for the for statement in this chapter to help you
     figure this out. Then test your prediction by trying out these lines in a
     program.

     ``python
     start
     end
     ``
### Programming Exercises

1. A user-friendly program should print an introduction that tells the user
what the program does. Modify the convert.py program (Section 2.2) to
print an introduction.
    
    ```python
    # convert.py
    #     A program to convert Celsius temps to Fahrenheit
    # by: Susan Computewell
    
    def main():
        print("This is a program that converts Celsius temperature into Fahrenheit")
        celsius = eval(input("What is the Celsius temperature? "))
        fahrenheit = 9/5 * celsius + 32
        print("The temperature is", fahrenheit, "degrees Fahrenheit.")
    
    main()
    ```

2. On many systems with Python, it is possible to run a program by simply
clicking (or double-clicking) on the icon of the program file. If you are
able to run the convert .py program this way, you may discover another
usability issue. The program starts running in a new window, but as soon
as the program has finished, the window disappears so that you cannot
read the results. Add an input statement at the end of the program so
that it pauses to give the user a chance to read the results. Something like
this should work:
input ("Press the <Enter> key to quit.")

    ```python
    print("This is a program to convert Celsius temps to Fahrenheit")
    celsius = eval(input("What is the Celsius temperature? "))
    fahrenheit = 9/5 * celsius + 32
    print("The temperature is", fahrenheit, "degrees Fahrenheit.")
    key = input("Press the <Enter> key to quit.")
    ```

3. Modify the avg2.py program (Section 2.5.3) to find the average of three
exam scores.
    
    ```python
    # avg2.py
    #   A simple program to average two exam scores  
    #   Illustrates use of multiple input
    
    def main():
        print("This program computes the average of three exam scores.")
    
        score1, score2, score3 = eval(input("Enter three scores separated by a comma: "))
        average = (score1 + score2 + score3) / 3
    
        print("The average of the scores is:", average)
    
    main()
    ```

4. Modify the convert.py program (Section 2.2) with a loop so that it executes 5 times before quitting. Each time through the loop, the program
should get another temperature from the user and print the converted
value.

    ```python
    # convert.py
    #     A program to convert Celsius temps to Fahrenheit
    # by: Susan Computewell
    
    def main():
        print("This is a program to convert Celsius temps to Fahrenheit")
        for x in range(5):
            celsius = eval(input("What is the Celsius temperature? "))
            fahrenheit = 9/5 * celsius + 32
            print("The temperature is", fahrenheit, "degrees Fahrenheit.")
    
    main()
    ```
5. Modify the convert.py program (Section 2.2) so that it computes and
prints a table of Celsius temperatures and the Fahrenheit equivalents every
10 degrees from 0°C to 100°C.

    ```python
    def main():
        print("Celsius     Fahrenheit")
        print("======================")
        for celsius in [0,10,20,30,40,50,60,70,80,90,100]:
            fahrenheit = 9.0 / 5.0 * celsius + 32
            print(celsius,"         ",fahrenheit)
       
    main()
    ```

6. Modify the futval.py program (Section 2.7) so that the number of years
for the investment is also a user input. Make sure to change the final
message to reflect the correct number of years.

```python
# futval.py
#    A program to compute the value of an investment
#    carried 10 years into the future

def main():
    print("This program calculates the future value")
    print("of an n-year investment.")

    principal = eval(input("Enter the initial principal: "))
    n_year = eval(input("Enter the number of years for the investment: "))
    apr = eval(input("Enter the annual interest rate: "))

    for i in range(n_year):
        principal = principal * (1 + apr)

    print(f"The value in {n_year} year/s is:", principal)

main()
```

7. Suppose you have an investment plan where you invest a certain fixed
amount every year. Modify `futval.py` to compute the total accumulation
of your investment. The inputs to the program will be the amount to invest
each year, the interest rate, and the number of years for the investment.

**There are two possible answers since the question did not specify whether to apply the apr before or after the fixed annual payment.**
```python
def main():
    print("This program calculates the future value of a yearly investment")
    print()

    payment = eval(input("Enter amount to invest each year: "))
    apr = eval(input("Enter the annualized interest rate: "))
    years = eval(input("Enter the number of years: "))

    principal = 0.0
    for i in range(years):
        principal = (principal + payment) * (1 + apr)

    print("The amount in", years, "years is:", principal)


main()

# futval.py
def main_two():
    print("""This program calculates the future value of an n-year investment where a fixed amount is added to the investment per year.""")

    annual_payment = eval(input("Enter amount to invest per year: "))
    n_year = eval(input("Enter a non-negative integer for the number of years for the investment to grow: "))
    apr = eval(input("Enter the annual interest rate: "))

    total = annual_payment
    for year in range(n_year):
        total = total * (1 + apr)
        total = total + annual_payment

    print(f"The value in {n_year} year/s is:", total - annual_payment)


main_two()
```


8. As an alternative to APR, the interest accrued on an account is often described in terms of 
a nominal rate and the number of compounding periods. For example, if the interest rate is 3% 
and the interest is compounded quarterly, the account actually earns 3/4% interest every 3 months.
<br></br>
Modify the `futval.py` program to use this method of entering the interest rate. 
The program should prompt the user for the yearly rate (rate) and the number of 
times that the interest is compounded each year (periods). To compute the value in 
ten years, the program will loop 10 * periods times and accrue rate/period interest on each iteration.

```python
# futval.py
#    A program to compute the value of an investment
#    carried 10 years into the future

def main():
    print("This program calculates the future value")
    print("of a 10-year investment.")

    principal = eval(input("Enter the initial principal: "))
    rate = eval(input("Enter the annual interest rate: "))
    periods = eval(input("Enter the number of times taht the interest is compounded each year"))

    
    for i in range(10 * periods):
        principal = principal * (1 + (rate/periods))

    print("The value in 10 years is:", principal)

main()

```

12. Write an interactive Python calculator program. The program should allow
the user to type a mathematical expression, and then print the value of the
expression. Include a loop so that the user can perform many calculations
(say, up to 100). Note: To quit early, the user can make the program
crash by typing a bad expression or simply closing the window that the
calculator program is running in. You'll learn better ways of terminating
interactive programs in later chapters.

```python
# An interactive Python Program that emulates a calculator.

def main():
    
    print("Hello, I am a calculator.")
    print("Give me an expression and I'll try to find its value")
    
    for i in range(100):
        expression = eval(input("What is the expression?"))
        print(expression)

main()
```