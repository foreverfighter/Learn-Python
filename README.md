# Learn-Python
_Learn/practise Python hands-on by following these exercises in the interpreter._

Get Python and the interpreter [**here**](https://www.python.org/downloads/).

### Instructions for use
_Open the interpreter, type a line of code, press enter and observe the output._

_For indented lines, use a tab for each indent._

#### 1.0 Basic Data Types
```python
print('Hello World')
print('Henry's shoelace')
print('Henry\'s shoelace')
print('Henry\'s\nshoelace')

print("""This
is
my
multiline
string""")

'Humpty ' + 'Dumpty'
'Ice ' * 2 + 'Baby'
5 + ' Fingers' #gives error
str(5) + ' Fingers'
'5' + 5 #gives error

2 + 2
2.0 + 2
2 - 1
3 * 2
3 / 2
5 ** 2
11 // 2
11 % 2

int('5') + 5
float('2') + 2
```
**Terms to Learn**
Console, Data Type, Strings, Integer, Escape, Operations, Type Conversion, Float

#### 1.1 Variables
```python
x = 5
x
dir()
x = x + 1
x
del x
x

x = 5
x++
x
x += 1
x
x -= 1
x
x *= 3
x

x = input() # type 'Monty'
y = 'Python'
z = x + y
z = x + ' ' + y
dir()
```
**Terms to Learn**
Variable, Declaration, Assignment, Increment, In-Place Operations, Namespace

#### 1.2 Lists, Ranges
```python
ls = []
ls
ls = [1,2,3,4,5,6,7]
ls

ls[0]
ls[2]
ls[-1]

ls[2:]
ls[1:-1]
ls[2:5]
ls[:5]
ls[2:]
ls[::-1]

4 in ls

len(ls)

ls.append(10)
ls
ls.insert(3,8)
ls
ls.index(8)
ls.index(10)
ls.remove(8)
del ls[2]
ls

range(7)
list(range(7))
list(range(2,9))
list(range(2,19,3))
```
**Terms to Learn**
List, Index, Element, Append, Remove, Range, List Slice

#### 1.3 Booleans, If Statements
```python
x = 15
x == 15
x == 10
x != 10
x != 15
x > 10
x >= 15
x > 10 and x > 13
x > 10 and x > 16
x > 10 or x > 16
not x > 10

x = 15
if (x == 15):
  print('x is 15')
  elif (x > 15):
    print('x is greater than 15')
  else:
    print('x is less than 15')

x = 15
not x
not not x
x = 0
not not x
x = [5]
not not x
x.remove(5)
not not x
x = 'word'
not not x
x = ''
not not x

if x:
  print('x is Truthy!')
  else:
    print('x is Falsy!')
```
**Terms to Learn**
Boolean, Truthiness, If Statement, Expression

#### 1.4 Loops
```python
for i in range(5):
  print(i)

i = 0
while i < 7:
  print(i)
  i++

i = 0
while i < 7:
  print(i)
  i++
  if (i == 5):
    break

i = 0
while i < 7:
  i++
  if (i == 5):
    continue
  print(i)

pokemons = ['Squirtle', 'Charmander', 'Bulbasaur']
for pokemon in pokemons:
  print(pokemon)
```
**Terms to Learn**
For Loop, Iterable, While Loop

#### 2.0 Functions
```python
def my_func():
  print('This is my function')
my_func()

def my_func():
  return 5
3 + my_func()

def my_func():
  return 5
  print('This is my function') # not printed because it's after the return statement
3 + my_func()

def square(x):
  return x**2
square(5)

def exponent(x, y):
  return x**y
exponent(5,3)

x = 5
def change_x(arg):
  x = arg
  print(x)
  y = 50
change_x(10)
x
y
dir()
```
**Terms to Learn**
Function, Definition, Call, Return, Parameter, Argument, Global Scope, Local Scope

#### 2.1 Modules
```python
import random
random.randint(1,100)

from random import randint
randint(1,100)

from random import * # imports all functions from the module and removes the need for [random.], not recommended
x = list(range(10))
shuffle(x) # this is a function from the module random

$pip install requests
```
**Terms to Learn**
Script, Module, Library, Standard Library, Import, pip, pypi

#### 2.2 Exceptions
```python
try:
  x = int(input('Enter a number: '))
except:
  print('Invalid input')
else:
  print('Entered ' + x)

x = 5
assert x < 4, 'x is not less than 4'
```
**Terms to Learn**
Try Block, Exception

#### 2.3 File Manipulation
```python
with open('my_file.txt','w') as f:
  f.write('my text to write to file') # check the directory you were in when you started python for the my_file.txt you just created

with open('my_file.txt','w') as f:
  f.write('this is more text to write') # check my_file.txt again

with open('my_file.txt','a') as f: # the 'a' will let us add on to the old text instead of overwriting
  f.write('\nI am now adding new text')

with open('my_file.txt') as f:
  cont = f.read()
print(cont)

with open('my_file.txt') as f:
  cont = f.readlines()
print(cont)
```
**Terms to Learn**
With, Open, Write, Append, Read

#### 2.4 Dictionaries, Tuples
```python
x = {'Name': 'Stitch', 'Species': 'Monster', 'Age':7}
x['Name']
x.keys()
x.values()
'Species' in x
'Monster' in x # 'in' only checks keys and not values

x = 1,2,3,4,5
x
x[0]
x = ()
x
```
**Terms to Learn**
Dictionary, Key, Value, Access, Tuple

#### 2.5 chr()/ord()/.split()/.join()/.format()
```python
for i in range(65,90):
  print(chr(i))

for i in 'abcdefgh':
  print(ord(i))

x = 'this is sparta'
x.split(' ')

x = ['Mickey','Donald','Bugs']
', '.join(x)

'{} cuts deeper than {}'.format('fear','swords')
```
**Terms to Learn**
ASCII

#### 2.6 Classes
```python
class Car:
  def __init__(self):
    self.wheels = 4
    self.speed = 60
    self.condition = 2
    self.model = 'Unspecified'
  def drive(self):
    if self.condition:
      print('Vroom!')
      self.condition -= 1
    else:
      print('The car needs to be repaired!')
  def repair(self):
    print('Repaired the car!')
    self.conditon = 2

my_car = Car()
my_car.speed
my_car.drive()
my_car.drive()
my_car.drive()
my_car.repair()

class Ferrari(Car):
  def __init__(self):
    super().__init__()
    self.model = 'Ferrari'
  def drive(self):
    print('Vroooooooommm!!!')
    self.condition -= 1

my_fer = Ferrari()
my_fer.wheels
my_fer.drive()
my_fer.drive()
my_fer.drive()
my_fer.repair()
```
**Terms to Learn**
Object-Oriented Programming, Class, Definition, Instantiation, Method, Dunder, Init, Inheritance, Attribute

#### 3.0 List Comprehensions
```python
r = range(10)
r
lc = [i*2 for i in r]
lc
lc = [i**2 for i in r]
lc
lc = [i for i in r where i%2 == 0]
lc
```
**Terms to Learn**
List Comprehension

#### 3.1 Script Conventions
```python
/#!/usr/bin/env python3

class MyClass:
  '''Short explanation of the class and its purpose'''

  def __init__(self):
  '''Short explanation of the constructor and its usage'''
    # constructor code here

  def my_method(self):
  '''Short explanation of the method and its usage'''

def main():
  # your script's code here

if __name__ == '__main__':
  main()
```
**Terms to Learn**
Shebang