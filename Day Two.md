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
str1.lower()
str1.upper()
str1.swapcase()  :  Uppercase to lowercase and lowercase to uppercase.
str1.capitalize() : Capitalize the first letter
str1.title() : capitalize the first letter of every words
str1.rjust() 
str1.zfill()

