# Learn-Python
_Follow these exercises in a jupyter notebook._
or on Mu! https://codewith.mu/en/download

# 1.0 Basic Data Types
```python
'Hello World'

'Humpty ' + 'Dumpty'
'Ice ' * 2 + 'Baby'
5 + ' Fingers'
str(5) + ' Fingers'
'5' + 5

2 + 2
2.0 + 2
2 - 1
3 * 2
3 / 2
5 ** 2
30 // 4
25 % 10

int('5') + 5
float('2') + 2
```
**Terms to Learn**
Data Type, Strings, Integer, Float, Type Conversion

# 1.1 Variables
```python
n = 5
n

n = n + 1
n

start = 'Python is'
times = 2
part_to_multiply = ' Very'
end = ' Awesome'

start + times * part_to_multiply + end

# Naming variables
```
**Terms to Learn**
Variable, Declare, Assign

# 1.2 Lists, Ranges
```python
[]

ls = ['a', 'b', 'c', 'd', 'e', 'f', 'g']
ls

ls[0]
ls[2]
ls[-1]

ls[2:]
ls[:5]
ls[2:5]

4 in ls

len(ls)

ls.append(10)
ls

ls.remove(8)
ls

range(7)
list(range(7))
list(range(2, 9))
```
**Terms to Learn**
List, Access, Index, Element, Append, Remove, Range, List Slice

# 2.4 Dictionaries
```python
x = {'Name': 'Stitch', 'Species': 'Monster', 'Age': 7}
x['Name']
x.keys()
x.values()
'Species' in x
'Monster' in x  # 'in' only checks keys and not values
```
**Terms to Learn**
Dictionary, Key, Value, Access

# 1.3 Booleans, If Statements
```python
x = 15
x == 15
x == 10
x != 10
x != 15

x = 15
if x == 15:
    print('x is 15')
elif x > 15:
    print('x is greater than 15')
else:
    print('x is less than 15')
```
**Terms to Learn**
Boolean, If Statement

# 1.4 Loops
```python
for i in range(5):
    print(i)

i = 0
while i < 7:
    print(i)
    i += 1

i = 0
while i < 7:
    print(i)
    i += 1
    if i == 5:
        break

i = 0
while i < 7:
    i += 1
    if i == 5:
        continue
    print(i)

pokemons = ['Squirtle', 'Charmander', 'Bulbasaur']
for pokemon in pokemons:
    print(pokemon)
```
**Terms to Learn**
For Loop, Iterable, While Loop

# 2.0 Functions
```python


def my_func():
    print('This is my function')


my_func()


def my_func():
    return 5


3 + my_func()


def my_func():
    return 5
    print('This is my function')  # not printed because it's after the return statement


3 + my_func()


def square(x):
    return x**2


square(5)


def exponent(x, y):
    return x**y


exponent(5, 3)

x = 5


def change_x(arg):
    x = arg
    print(x)
    y = 50


change_x(10)
x
y
```
**Terms to Learn**
Function, Definition, Call, Return, Parameter, Argument, Global Scope, Local Scope

# 2.1 Modules
```python
import random
random.randint(1, 100)

from random import randint
randint(1, 100)

from random import *  # imports all functions from the module and removes the need for [random.], not recommended
x = list(range(10))
shuffle(x)  # this is a function from the module random

$pip install requests
```
**Terms to Learn**
Script, Module, Library, Standard Library, Import, pip, pypi

# 2.3 File Manipulation
```python
with open('my_file.txt', 'w') as f:
    f.write('my text to write to file')  # check the directory you were in when you started python for the my_file.txt you just created

with open('my_file.txt', 'w') as f:
    f.write('this is more text to write')  # check my_file.txt again

with open('my_file.txt', 'a') as f:  # the 'a' will let us add on to the old text instead of overwriting
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

# 2.5 .format()
```python
'{} cuts deeper than {}'.format('fear', 'swords')
```

# 2.6 Classes
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
        self.condition = 2


my_car = Car()
my_car.speed
my_car.drive()
my_car.drive()
my_car.drive()
my_car.repair()
```
**Terms to Learn**
Class, Define, Instantiate, Method, Init, Attribute
