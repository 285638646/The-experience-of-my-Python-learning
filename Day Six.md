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
