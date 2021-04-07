## String
String is any text enclosed in single or double quotes. Once you define a sring , it can't be changed.

str1 = ' Python is the best language in the world. '
str2 = " Does not support rebuttal. "

## String operations

String is supported to plus and multiply.

```

print(str1 + str2)
Python is the best language in the world.  Does not support rebuttal. 

print(str1 * 3)
Python is the best language in the world.  Python is the best language in the world.  Python is the best language in the world. 

```

## Find characters by index

str1 = 'Python is the best language in the world. '

```
print (str1 [2] )
t

print(str1 [2:5])
tho

print(str1 [:5] )
Pytho

print(str1 [2:])
thon is the best language in the world. 

print("is" in str1)
true

print("is"  not in str1)
false

attention：Space is also counted as one character

```

## Bitwise negation

~9 结果：-10
Original code ：00001001
Inverse code：11110110
Complement code：10001001
Correction：10001010 1是负，加1修正
Conversion：-0008020 -> 10
 
~-9 结果：8
Original code：10001001
Inverse code：01110110
Complement code：00001001
Correction：00001000 0是正，减1修正
Conversion：+0008000 -> 8
 
Regulation：~num=-(num+1)


## Formatted output

print("num =" , num )
print("num = %d , str1 = %.3f " % (num , str1))

```
num = 2
str1 = 0.3
print("num = %d , str1 = %.3f " % (num , str1))
```
## ESC : escape character
line break : \n
tbs : \t

print(r"\\\t\\")
sometimes we use r"" to not escape the character in brakets. 

##

print(eval(" 12+3 "))
len()
str.lower()
str.upper()
str.swapcase()  :  Uppercase to lowercase and lowercase to uppercase.
str.capitalize() : Capitalize the first letter
str.title() : capitalize the first letter of every words
str.rjust() 
str.zfill()
str.count(str[,start][,end])
str.find(str[,start][,end])
str.index(str[,start][,end])
str.rindex（）
str.lstrip()
str.rstrip()
str.strip()

# statement while

while expression:
     sentence
     else:
     expression
```

num = 1
sum = 0
while num <= 100:
    sum += num
    num += 1
else:
    print(sum)

```

```

num = 100
total = 0
while num < 1000:
    a = num % 10
    b = num // 10 % 10
    c = num // 100
    if a**3 + b**3 + c**3 == num:
        total += 1
        print(num)
        num += 1
    else:
        num +=1
else:
    print("there are %d number of daffodils." % total)

```

```
num = 10000
total = 0
while num < 100000:
    num = str(num)
    if num[4] == num[0] and num[3] == num[1]:
        total += 1
        num = int(num) + 1
    else:
        num = int(num) + 1

else:
    print("there are %d palindromic numbers." % total)
```

```
num = int(input("Please input a number:"))
i = 2
while i < num:
    if num % i == 0:
        print ("%d is not a prime number." % num)
        i += 1
        break
    else:
        i += 1
else:
    print("%d is a prime number." % num)
```

```

num = 3
i = 2
a = [1,2]
while num < 1000:
    if i < num :
            if num % i == 0:
               num += 1
               i = 2
            else:
               i += 1
    else:
        a.append(num)
        num += 1
        i = 2
#else:
   # print(a)


pro = int(input("plese input a number:"))
b = [1]
j = 1
c = a[j]
while j <= pro:
    if  pro % c == 0:
        b.append(c)
        pro /= c
        j = 1
        c = a[j]
    else:
        j += 1
        c = a[j]
else:
   k = 0
   d = len(b)
   pro = int(pro)
   while k < d:
       pro *= b[k]
       k += 1
   else:
    print("The prime factor of %d is %s " % (pro,b))
    
 ```

