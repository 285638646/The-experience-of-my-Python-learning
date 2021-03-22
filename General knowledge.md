## Number of daffodils
The number of daffodils refers to a 3-digit number, and the sum of the digits to the power of 3 is equal to itself.

```

num = int(input("please input a 3-digit number："))
a = num % 10
b = num // 10 % 10
c = num % 100
if num == a**3 + b**3 + c**3 :
    print("It is a number of daffodils")
else:
    print("It is not a number of daffodils")
    
```

## Palindrome Number
The result of a number read from the left and read from the right is exactly the same, such as 12321.

```

num = int(input("please input a 5-digit number："))
a = num % 10
b = num // 10  % 10
c = num // 100 % 10
d = num // 1000 % 10
e = num // 10000
if a == e and b == d :
    print("It is a Palindrome Number")
else:
    print("It is not a Palindrome Number")

```
