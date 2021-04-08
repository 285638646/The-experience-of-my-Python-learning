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
