# Python Functions :space_invader:	

### Learning Objectives
*By the end of this module you should be able to answer the following:* :grin:

*
*

### Functions Introduction

In Python, a function performs a certain task. It usually involves taking some input, manipulating the input and returning an output.

This named section of a code is a block of organized reusable code. This trait is extremely important as our program grows larger and larger, as it makes our code more **organized** and **manageable**.

## Example Problems :nerd_face:	

### Problem 1: Create a function in Python
Write a program to create a function that takes two arguments, name and age, and print their value.

**Hint:** 

* Use the def keyword with the function name to define a function.
* Next, take two parameters
* Print them using the print() function
* Call function by passing name and age.

**Solution:**
```python
#data is the fuction name
def data(name, age):
  # print value
    print(name, age)

# call function
data("Jamie", 21)
```

### Problem 2: Create a function with variable length of arguments
Write a program to create function ```set()``` to accept a variable length of arguments and print their value.

**Note:** Create a function in such a way that we can pass any number of arguments to this function and the function should process them and display each argument’s value

**Given:**
```
# call function with 3 arguments
set(20, 40, 60)

# call function with 2 arguments
set(80, 100)
```

**Expected Output:**
```
20
40
60
80
100
```
**Hint:**
To accept a variable length of positional arguments, i.e., To create functions that take n number of positional arguments we use *args as a parameter. (prefix a parameter name with an asterisk * ).

**Solution:**
```python
def set(*args):
    for i in args:
        print(i)

set(20, 40, 60)
set(80, 100)
```
### Problem 3: Return multiple values from a function
Write a program to create function ```calc()``` such that it can accept two variables and calculate **addition** and **subtraction**. Also, it must return both addition and subtraction in a single return call.

**Given:**
```python
def calc(a, b):
    # Your Code

ans = calculation(50, 40)
print(res)
```
**Expected Output:**
```
(90, 10)
```
**Hint:**
Separate return values with a comma.

**Solution:**
```python
def calc(a, b):
    add = a + b
    subtract = a - b
    # return multiple values separated by comma
    return add, subtract

ans = calc(50, 40)
print(ans)
```

### Problem 4: Create a function with default argument
Write a program to create a function ```show_employee()``` using the following conditions.

* It should accept the employee’s name and salary and display both. 
* If the salary is missing in the function call then assign default value **24000** to salary

**Given:**
```python
showEmployee("Nafis", 121000)
showEmployee("Max")
```

**Expected Output:**
```
Name: Ben salary: 121000
Name: Jessa salary: 24000
```

**Hint:**
Default arguments take the default value during the function call if we do not pass them. We can assign a default value to an argument in function definition using the = assignment operator.

**Solution:**
```python
def show_employee(name, salary=24000):
    print("Name:", name, ", Salary:", salary)

show_employee("Nafis", 121000)
show_employee("Max")
```

## Practice Questions :yawning_face:	

### Practice Question 1: Create a recursive function
Write a program to create a recursive function to calculate the sum of numbers from 0 to 500.

A recursive function is a function that calls itself, again and again.

**Expected Output:**
```
125250
```
### Practice Question 2: Assigning new names to functions
Write a function called ```display_name(name, age)```. 
Rename it ```new_name(name, age)``` and call the new assigned name

You should be able to call the previous function using ```new_name(name, age)```



### Practice Question 3: Creating function with simple arguments
Write a function that takes a person's name and year of birth and displays in ```candidate(name, yyyy)``` 


**Expected Output**
```
Name: Nafis YOB: 2005
```
### Practice Question 4
Given a list of integers, return ```True``` if the array contains a 7 next to a 7 somewhere.

```python
num([1, 7, 7]) → True
num([1, 7, 1, 7]) → False
num([7, 1, 7]) → False
```

## Challenge Question
Write a function that uses a list of integers and returns ```True``` if it contains ```9, 8, 1``` in order.

```python
set([5,2,4,9,8,1,5]) --> True
set([9,8,1,4,0,5,7]) --> True
set([9,7,2,4,4,5,2]) --> False
```
