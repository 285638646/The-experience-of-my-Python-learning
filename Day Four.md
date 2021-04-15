## Tuple

tuple = (1,)
tuple1 = (1,2,3,4,5)
tuple[0] = 1
tuple[-1] = 5

attention: the element in tuple can't be changed.
## operation
tuple = (1,2,3)
tuple1 = (4,5,6)
del tuple
addition subtraction multiplication 
print( 4 in tuple1)
print(tuple[1:2])
print(tuple[1:])
print(tuple[:2])

len()
max()
min()
split(str)
splitlines()
"",join()
replace(old,new,count)
maketrans()
translate()
startwith()
endwith()
encode()
decode()
isalpha()
isalnum()
isupper()
islower()
istitle()
isdigit()
isnumeric()
isdecimal()
isspace()


## dictionary

The dictionary us key-value to store data.

The key shouled be unique and unchageble.

dic{"tom":60}

dic["tom"]

dic.get()
dic["Adai"] = 80
dic.pop()
dic.values()
dic.items()

for k,v in dic.items()
   print(k,v)
   
for i, v2 in enumerate():
    print(i,v2)

```

address = input("please enter the lyric file address :")
name = input("please enter the name of the lyric file :")
form = input("please enter the form of the lyric file :")
open_address = address + "\\" + name + "." + form
File = open(open_address, "r")
# example : File = open(r'C:\Users\lenovo\Desktop\华语群星 - 北京东路的日子.lrc', "r")
Lyric = File.read()
File.close()
# Importing files

Lyric = Lyric.replace(']','] ')
Lyric = Lyric.replace('[',' [')
Lyric = Lyric.replace('-','')
Lyric = Lyric.replace('\n','')
Lyric = Lyric.replace('  ',' ')
Lyric = Lyric.split(' ')
del Lyric[0]
# Split file into strings

key = ""
value = ""
dic = {}
i = 0
j = 1
# Set initial value

while i in range(0,len(Lyric)-1):
    if Lyric[i][1] == '0':  # Determine if it is a timestamp like [00:00,00]
        key = Lyric[i]
        while Lyric[i+j][1] != '0' and i+j in range(0,len(Lyric)-1):
            value += "  "
            value += Lyric[i+j]  # If it is not a timestamp like [00:00,00] ,then it is Lyric.
            value = value.replace(" ","",1)
            j += 1
        else:
            dic.update({key: value}) # add the Key and Value to the dictionary
            i += 1
            if i == len(Lyric) - 1 and Lyric[len(Lyric) - 1][1] != '0': # The above method can't judge the last element.
                value += "  "                                           # So make additional judgments
                value += Lyric[len(Lyric) - 1]
                value = value.replace(" ", "", 1)
                dic.update({key: value})
            else:
                pass
    else:
        value = ""
        j = 1
        i += 1
else:
    time = list(dic.keys())
    t = input("please enter time like [12:34.56] : ")
    k = 0
    num = 0
    # The following method is used to determine whether the input meets the requirements
    while k in range(0,len(t)):
        if ord(t[k]) in range(48,58):
            num += 1
            k += 1
        else:
            k += 1
    else:
        while num != 6 or t[0] != "[" or t[len(t)-1] != "]": # The input must be six digits , and begin with [ ,end with ].
            print("Incorrect input.")
            t = input("please enter time like [12:34.56] : ")
            k = 0
            num = 0
            while k in range(0, len(t)):
                if ord(t[k]) in range(48, 58):
                    num += 1
                    k += 1
                else:
                    k += 1
        else:
            print("Entered correctly.")
    l = time[0]
    x = 0
    while t > max(time):  # when time is bigger than max(time) , there should be no Lyric.
        print("but song is over")
        t = input("please enter another time like [12:34.56] : ")
        k = 0
        num = 0
        while k in range(0, len(t)):
            if ord(t[k]) in range(48, 58):
                num += 1
                k += 1
            else:
                k += 1
        else:
            while num != 6 or t[0] != "[" or t[len(t) - 1] != "]":
                print("Incorrect input.")
                t = input("please enter time like [12:34.56] : ")
                k = 0
                num = 0
                while k in range(0, len(t)):
                    if ord(t[k]) in range(48, 58):
                        num += 1
                        k += 1
                    else:
                        k += 1
            else:
                print("Entered correctly.")
        l = time[0]
        x = 0
    else:
        while x in range(0,len(time)): # judge the nearest timestamp.
            if  time[x] < l and time[x] > t:
                l = time[x]
                x += 1
            else:
                x += 1
        else:
            print("The lyrics at this time are",dic[l])
           
```

## Function


