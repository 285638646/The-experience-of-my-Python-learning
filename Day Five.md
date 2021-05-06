# file handing
## open file
open(path,flag[,encoding],[errors])

flag : Open method
r  rb  r+  w  wb  w+  a  a+

encoding : encoding form  utf - 8
errors  : error handing ignore

## read file

filename.read(number)
filename.readline()  # include line break
filename.readlines()
filename.seek()

## close file
filename.close()

with open() as filename:


## write file

filename.write()
filename.flish()

## encode and decode

filename.encode()
filename.decode()


import pickle


pickle.dump(filename,f)
pickle.load(filename)


## OS module

os.name()
os.uname()
os.environ()
os.environ.get()
os.curdir()
os.getcwd()
os.mkdir()
os.listdir()
os.rmdir()
os.stat()
os.remove()
os.system("order sentence")  : notpad , write , mspaint ,msconfi 

os.path
os.path.join(path1,path2)
os.path.split()
os.path.isdir()
os.path.isfile()
os.path.getsize()
os.path.exists()
os.path.dirname()
os.path.basename()


## window control

[method](https://blog.csdn.net/qq_23934063/article/details/79584525)

## Memory modification

[method](https://www.cnblogs.com/pygo/p/12274652.html)
