# Learn-Python
_Learn/practise Python hands-on by following these exercises in the interpreter._

Get Python and the interpreter [**here**](https://www.python.org/downloads/).

### Instructions for use
_Open the interpreter, type a line of code, press enter and observe the output._

* quit()
* print('my string')
* 2 + 2
* 2 + 2 #this is a comment for humans to read
* 2.0 + 2
* 2 - 0
* 3 * 2
* 3 / 2
* 3 ** 2
* 9 // 2
* 9 % 2
* print('Henry's shoelace')
* print('Henry\'s shoelace')
* print('Henry\'s\nshoelace')
* input()
* 'Humpty ' + 'Dumpty'
* 'Ice ' * 2 + 'Baby'
* 5 + ' Fingers' #gives error
* str(5) + ' Fingers'
* '5' + 5 #gives error
* int('5') + 5
* float('2') + 2
* x = 5
* x
* del x
* x
* x = 5
* x += 1
* x
* x -= 1
* x
* x *= 3
* x
* x == 15
* x == 10
* x != 10
* x != 15
* x > 10
* x >= 15
* x < 10
* x <= 15
* if (x == 15):
  * print('x is 15')
  * elif (x > 15):
    * print('x is greater than 15')
  * else:
    * print('x is less than 15')
* x > 10 and x > 13
* x > 10 and x > 16
* x > 10 or x > 16
* not x > 10
* i = 0
* while i < 7:
  * print(i)
  * i += 1
* while i < 7:
  * print(i)
  * i += 1
  * if (i == 5):
    * break
* while i < 7:
  * print(i)
  * i += 1
  * if (i == 5):
    * break
* while i < 7:
  * i += 1
  * if (i == 5):
    * continue
  * print(i)
* my_list = []
* my_list
* my_list = [1,2,3,4,5]
* my_list[0]
* my_list[2]
* 4 in my_list

len(my_list)

my_list.append(10)

my_list

my_list.insert(3,8)

my_list

my_list.index(8)

my_list.index(10)

my_list.remove(8)

range(7)

list(range(7))

list(range(2,9))

list(range(2,19,3))

    for my_item in range(5):

        print(my_item)
.

    def my_function():

        print('This is my function')
.

    def my_function():

        return 5
.

    def my_function():

        return 5

        print('This is my function') # this doesn't get printed because it's after the return statement
.

3 + my_function()

    print("""This

    is

    my

    multiline

    string""")

import random


#### here are some interesting leads that these exercises do not cover

* standard libraries other than random
* regular expressions

#### to add on

import {}

random.randint(x,y)

from {} import {} as {}

from {} import *

try: except:

assert {statement}, {comment}

file = open()

file.close

cont = file.read()

file.readlines()

file.write()

with open('test.txt', 'a') as myfile:

{key:value,key:value}

dict[key] = value

key in dict

.get(key,[nokeycomment])

(x,y,z)

x,y,z

mylist[1:5:2]

[…for x in range(5) if ...]

ord()

chr()

.isalpha()

.translate()

split()

lambda x: x**2

map(function, iterable)

filter(function, iterable)

yield

set()

.add

.remove

.pop

'.'

'..'

if __name__ == '__main__':

#!/usr/bin/python

'''…'''

%c

%s

%d

%.

__attribute

def func(self):

def __init__(self):

{}

(?P<name>...)

(?:...)

|

class subc(class):

def __add__(self,other):

.format

@classmethod

@property

@myproperty.setter

@myproperty.deleter

*args

**kwargs
