## Notes
1. We use # to note single line.
2. We use ''' ''' or """ """ to note multi-line.

## Show your result on the screen
We use the 'print' function to display the date , text or symbol from your program.

``` 
print(12) 
print("Hello world")
print("#")   
```

Differ from the language C , you can use the 'print' function more smartly.

```
 print(1+2)  print(2*2)  print(6/2)
 print("Hello world" , "Hello Terry")
 print("#"*6)   print("10 + 8 =",18)
```

---

## Type your value to the program
We use the 'input' function to give the value artificially. And keep the value in the variables.

```
age = input(" 请输入您的年龄：")
print("your age is " , age)

```

---

## Data type

![image](https://github.com/285638646/The-experience-of-my-Python-learning/blob/Basic-Knowledge/Date%20type.png)


## Identifier

![image](https://github.com/285638646/The-experience-of-my-Python-learning/blob/Basic-Knowledge/Identifier.jpg)

## Number type

integer , float and complex number.

## Mathematical function

abs(x):Returns the absolute value of a number

```
a = -10
print(abs(a))
```

max(x,y):Returns the maximum value of a given parameter

```
print(max(1,2,3,4,5,6,7,8))

```

min(x,y):Returns the minimum  value of a given parameter


```
print(min(1,2,3,4,5,6,7,8))

```


pow(x,y):Find x to the power of y

```
print(pow(2,5))

```

round(float,digit):For rounding of floating point numbers

```
print(round(3.404,1))

```

import *Library Functions*

```
import math

print(math.ceil(19.9))
#Rounded up

print(math.floor(19.9)
#Rounded down

print(math.modf(22.3)
#Return the integer part and the float part

print(math.sqrt(16)
#square root
```

```
import random

print(random.choice([1,3,5,6,8]))
print(random.choice("random"))
#choose randomly

print(random.randrange(start,stop,step))
#The stop number is not including.

print(random.random())
#return a number randomly in [0,1).


random.shuffle(list)
#Randomly sort the data in the list

random.uniform(a,b)
#return a float number randomly in [a,b].

```

range(x):return an array conclude x number biginning from 0.

range(x) + 1:return an array conclude x number biginning from 1.

range(1,x+1):return an array conclude x number biginning from 1.


## Expression:A formula composed of variables , constants and operators.

Arithmetic Operator: + - * / % **  //
Arithmetic expression: 1 +2 2*3 a/3      * Perform related mathematical operations *
Value:The results obtained
Assignment operator: =
Compound operator： += -= *= /= %=  **= //=   a+=b

## Commonly used functions

if expression:
    sentence 1
else 
    sentence 2
    
   
function：Determine whether the given conditions are met, and decide to perform one of the two operations given according to the result of the determination (true or false)
    
```

x = int(input("please input a integer："))
if x % 2 == 0:
    print("It is an even number")
else:
    print("It is not an even number")

```

## Bitwise operator
 
& : Bitwise AND operator
| : Bitwise OR operator
^ : Bitwise exclusive OR operator
~ : Bitwise negation operator
#formula：-（a+1）
