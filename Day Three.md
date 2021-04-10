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
