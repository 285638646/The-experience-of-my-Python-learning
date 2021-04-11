## List

list = []
list = [1,2,3,4,5]
list = [1,2,3,"few"]

## Operation
you can add , subtract , multiply list.

print(3 in list)
print(list[2:3])

## Two dimensional list
list=[[1,2,3],[4,5,6],[7,8,9]]
print(list[1][1])

## function

list= []
list.append()
list.extend()
list.insert(location,addition)
list.pop()
list.remove()
list.clear()
list.index()
len()
max()
min()
list.count()
list.reverse()
list.sort()
list.copy()  Shallow copy and deep copy

## if elif eise

if expression:
   sentence
   elif expression:
    sentence
   else:
    sentence
    
```
import random

print("This is a quiz game.")
num = int(input("Please input a number : "))
random = random.randint(0,100)
while num != random:
    if num >= 101:
        print("The number is less than one hundred.")
        num = int(input("Try again. Please input another number : "))
    elif num > random:
        print("Too big")
        num = int(input("Try again. Please input another number : "))
    else:
        print("Too small")
        num = int(input("Try again. Please input another number : "))
else:
    print("Congratulations , this number is %d" % random)
```

Endless loop：Expression is always true.

## statament for

for variables in gather:
    sentence

```

for i in [1,2,3,4,]:
   print(i)
```

```
for index, m in enumerate([1,2,3,4,5]):
   print(index,m)
```

break
countinue

```
i = 1
j = 1
num = []
MT = []
while i < 10 :
    while j <= i:
        new = (" %d * %d = %d " % (i,j,i*j))
        num.append(new)
        j += 1
    else:
        MT.append(num)
        num = []
        j = 1
        i += 1
else:
    k = 0
    for k in range(0,9):
        print(MT[k])
```

```

print("Please input two number : ")
i = 0
inp = []
CD = []
while i < 2:
    inp.append(int(input()))
    i += 1
else:
    for j in range(1,max(inp)+1):
        if inp[0] % j == 0 and inp[1] % j == 0:
            CD.append(j)
            j += 1
        else:
            j += 1
    else:
        print(" The greatest common divisor of number %d and %d is %d " % (inp[0],inp[1],max(CD)))

```

```

str = input("please input a string : ")
i = 0
change = list(str)
while i in range(0,len(str)):
    if ord(str[i]) in range(65,91):
        change[i] = chr(ord(str[i])+32)
        i += 1
    elif ord(str[i]) in range(97, 123):
        change[i] = chr(ord(str[i])-32)
        i += 1
else:
    print(''.join(change))

```

```

import random
range1 = range(48,58)
range2 = range(65,91)
range3 = range(97,123)
sco = []
i=0
while i < 123:
    if i in range1:
        sco.append(i)
        i += 1
    elif i in range2:
        sco.append(i)
        i += 1
    elif i in range3:
        sco.append(i)
        i += 1
    else:
        i += 1
else:
    AC = []
    i = 0
    while i < 6:
        new = random.choice(sco)
        AC.append(chr(new))
        i += 1
    else:
        print(''.join(AC))

```

## function turtle

Coordinates of drawing origin: (0.0) , located in the middle of the screen , initial direction to the right.


Movement commands:
forward(d)
backward(d)
right(a)
left(a)
goto(x,y)
speed(s) : s in range(0,11)
up()
setheading(a)
pensize(w)
pencolor(cs)
reset()
clear()
circle(r,steps=e) : the r is radius and the e is  the number of size.
begin_fill()
fillcolor(cs)
end_fill()


control commands:

Other commands:
undo()
down()
hideturtle()
showturtle()
screensize(x,y)

```

```
import turtle
i = 0
initial = -72
while i in range(0,5):
    turtle.setheading(initial)
    turtle.forward(100)
    initial -= 144
    i += 1
else:
    turtle.hideturtle()
    turtle.done()

```

import turtle
x = int(input("please input the side length of square : "))
i = 0
while i in range(0,4):
    turtle.forward(x)
    turtle.right(90)
    i += 1
else:
    turtle.done()
```

```

import turtle
x = int(input("please input the side length of rectangle : "))
y = int(input("please input the side width of rectangle : "))
i = 0
while i in range(0,2):
    turtle.forward(x)
    turtle.right(90)
    turtle.forward(y)
    turtle.right(90)
    i += 1
else:
    turtle.done()

```

```

import math
import turtle
x = int(input("please input the side length of rectangle : "))
y = int(input("please input the side width of rectangle : "))
z = 5 * math.sqrt(int(input("please input the side height of rectangle : ")))
if x < y:
    x, y = y, x
i = 0
j = 0
k = 0
h = 0
while i in range(0,2):
    turtle.forward(x)
    turtle.right(90)
    turtle.forward(y)
    turtle.right(90)
    i += 1
else:
    turtle.goto(z, z)
    turtle.setheading(0)
    while j in range(0,2):
        turtle.forward(x)
        turtle.right(90)
        turtle.forward(y)
        turtle.right(90)
        j += 1
    else:
        while k in range(0,3):
            turtle.up()
            turtle.goto(h,-y)
            turtle.down()
            turtle.setheading(45)
            turtle.forward(z*math.sqrt(2))
            k += 1
            if h < x:
                h += x
            else:
                y = 0
        else:
            turtle.done()
```

```

import turtle

turtle.speed(0)
i = 0
x = 0
y = 0
z = -5
initial = -72
while i in range(0,5):
    turtle.circle(20)
    turtle.up()
    if i < 2:
        x += 25
        turtle.goto(x,0)
        turtle.down()
        i += 1
    else:
        z += 20
        y = -20
        turtle.goto(z,y)
        i += 1
        turtle.down()
else:
    turtle.done()
    
```

```

import turtle
turtle.speed(0)
i = j = 0
x = 0
y = 0
while i in range(0,19):
    x = 180
    turtle.goto(x,y)
    y += 10
    turtle.up()
    turtle.goto(0,y)
    turtle.down()
    i += 1
else:
    turtle.up()
    turtle.goto(0,0)
    turtle.down()
    x = 0
    while j in range(0,19):
        y = 180
        turtle.goto(x,y)
        x += 10
        turtle.up()
        turtle.goto(x,0)
        turtle.down()
        j += 1
    else:
        turtle.hideturtle()
        turtle.done()
```

```

import turtle
turtle.speed(0)
i = j = 0
k = 0
x = 0
y = 0
while i in range(0,8):
    while j in range(0,8):
        l = 0
        turtle.up()
        turtle.goto(x, y)
        turtle.down()
        if (k % 2) != 0:
            turtle.begin_fill()
            while l in range(0,4):
                turtle.forward(20)
                turtle.right(90)
                l += 1
            else:
                turtle.fillcolor("white")
                turtle.end_fill()
                k += 1
                j += 1
                x += 20
        elif k % 2 == 0:
            turtle.begin_fill()
            while l in range(0, 4):
                turtle.forward(20)
                turtle.right(90)
                l += 1
            else:
                turtle.fillcolor("black")
                turtle.end_fill()
                k += 1
                j += 1
                x += 20
    else:
        k += 1
        i += 1
        x = 0
        j = 0
        y += 20
else:
    turtle.hideturtle()
    turtle.done()
    
```
