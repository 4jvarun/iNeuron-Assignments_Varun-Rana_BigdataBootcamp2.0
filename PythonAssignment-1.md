## Assignment Part-1
Q1. Why do we call Python as a general purpose and high-level programming language?
Ans 
    Python is a user friendly language which let's the user do programming in a human readable format and the code is translated to a low level language via a compiler

Q2. Why is Python called a dynamically typed language?
Ans 
    Python is a dynamically typed language as the variable type is determined during runtime. The same variable can have different types at different times.

Q3. List some pros and cons of Python programming language?
Ans 
    Pros
    1	Flexible
    2	User friendly
    3	Scalable
    4	Extensive libraries
    5	Less coding

    Cons
    1	Security
    2	Dynamically typed
    3	Garbage collection
    4	Speed limitations
    5	Design restrictions


Q4. In what all domains can we use Python?
Ans 
    1	Machine learning / Artificial intelligence
    2	Desktop GUI
    3	Data analytics and data visualization 
    4	Web development
    5	Game development
    6	Mobile app development
    7	Embedded systems

Q5. What are variable and how can we declare them?
Ans 
    Variable is a name given to a memory location. A variable name starts with an alphabet and we can't use special symbols in a variable. We can declare a variable mentioned below:
    a = 2
    b = 3
    print(a+b)
    output-> 5

Q6. How can we take an input from the user in Python?
Ans 
    By using an inbuilt function from python libraries input()

Q7. What is the default datatype of the value that has been taken as an input using input() function?
Ans 
    The value returned by the input() is of a type string.

Q8. What is type casting?
Ans 
    Type casting is a method which is used to convert a one variable type to another for e.g. if we have:
    a = 5 # which is an integer values
    a.cast('float') # will change the value from integer value to a decimal value
    output-> 5.0

Q9. Can we take more than one input from the user using single input() function? If yes, how? If no, why?
Ans 
    Yes, a single input() function can be used to take more than one input from the userm, for e.g->
     x,y,z = input( ).split()

Q10. What are keywords?
Ans 
    Keywords define the syntax rules and structure of any language

Q11. Can we use keywords as a variable? Support your answer with reason.
Ans 
    Keywords define the syntax rules and structure of any language hence they cannot be used as variable names.

Q12. What is indentation? What's the use of indentaion in Python?
Ans 
    Indentation refers to the spaces at the beginning of a code line. Python uses indentation to indicate a block of code.

Q13. How can we throw some output in Python?
Ans 
    The basic way to do output is the print statement
    
    print('Hello') 
    output -> Hello

Q14. What are operators in Python?
Ans 
    Python Operators in general are used to perform operations on values and variables. There are different type of operators, given below:
    
    Arithmetic operators (+,–,*,/,//,%,**)
    Assignment operators (=,+=,-=,*=,/=,%=,//=,**=,&=,|=,^=,>>=,<<=)
    Comparison operators (>,<,==,!=,>=,<=,is,is not)
    Logical operators (and, or, not)
    Identity operators (is, is not)
    Membership operators (in, not in)
    Bitwise operators (&,|,~,^,>>,<<)

Q15. What is difference between / and // operators?
Ans 
    '/' is the division operator. '//' is the floor division operator.
    for e.g
    
    if x = 17,
       y = 3

    then
        x/y => output(5.67)
        x//y => output(5)

       if the quotient obtained by dividing two numbers is not an integer, then operators '/' and '//' will return different answers

Q16. Write a code that gives following as an output.
```
iNeuroniNeuroniNeuroniNeuron
```
Ans 
    print("iNeuron"*4)

Q17. Write a code to take a number as an input from the user and check if the number is odd or even.
Ans 
    a = input("Hello user, please enter a number \n")
    a = int(a)
    if a%2==0:
        print("This is an even number")
    else:
        print("This is an odd number")

Q18. What are boolean operator?
Ans 
    There are three logical operators that are used to compare values. They evaluate expressions down to Boolean values, returning either True or False . These operators are and , or , and not.

Q19. What will the output of the following?
```
1 or 0 

0 and 0 

True and False and True

1 or 0 or 0 
```
Ans 
    1 or 0 : Ans 1

    0 and 0 : Ans 0

    True and False and True : Ans False

    1 or 0 or 0 : Ans 1

Q20. What are conditional statements in Python?
Ans 
    if
    if, else.
    Nested if
    if-elif statements.

Q21. What is use of 'if', 'elif' and 'else' keywords?
Ans 
    'if' keyword-> The if condition helps make a decision based on whether the condition is true or not. 
    'else' keyword-> When we encounter a situation where you we several conditions, we can place as many elif conditions as necessary between the if condition and the else condition
    'else' keyword-> The logical decisions where the 'if' condition fails then we can simply add another condition, which is the else condition.

Q22. Write a code to take the age of person as an input and if age >= 18 display "I can vote". If age is < 18 display "I can't vote".
Ans
    age = int(input("Please enter your age to know eligibility for vote \n"))
    if age >= 18:
        print("I can vote")
    else:
        print("I can't vote")

Q23. Write a code that displays the sum of all the even numbers from the given list.
```
numbers = [12, 75, 150, 180, 145, 525, 50]
```
Ans 
    numbers = [12, 75, 150, 180, 145, 525, 50]
    lizt= []
    for num in numbers:
        if num%2==0:
            lizt.append(num)   
    sum_num = sum(lizt)
    print(sum_num)

Q24. Write a code to take 3 numbers as an input from the user and display the greatest no as output.
Ans 
    x,y,z = input('Hi user, please enter three different numbers seperated by a space \n').split()
    nos = [x,y,z]

    if nos[0]>nos[1] and nos[0]>nos[2]:
        print(nos[0]," is the greatest")
    elif nos[1]>nos[0] and nos[1]>nos[2]:
        print(nos[1]," is the greatest")
    else:
        print(nos[2]," is the greatest")


Q25. Write a program to display only those numbers from a list that satisfy the following conditions

- The number must be divisible by five

- If the number is greater than 150, then skip it and move to the next number

- If the number is greater than 500, then stop the loop
```
numbers = [12, 75, 150, 180, 145, 525, 50]
```
Ans 
    numbers = [12, 75, 150, 180, 145, 525, 50]

    lizt = []

    for x in numbers:
        if x > 150:
            continue
        elif x%5==0:    
            lizt.append(x)  
        elif x>500:
            break

    print("Numbers divisible by 5 = ",lizt)