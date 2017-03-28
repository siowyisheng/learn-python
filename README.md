# Learn-Python
_Learn/practise Python hands-on by following these exercises in the interpreter._

Get Python and the interpreter [**here**](https://www.python.org/downloads/).

### Instructions for use
_Open the interpreter, type a line of code, press enter and observe the output._

_For indented lines, use a tab for each indent._

#### 1.0 Basics
* quit()
* print('my string')

#### 1.1 Strings
* print('Henry's shoelace')
* print('Henry\\'s shoelace')
* print('Henry\\'s\nshoelace')
* print("""This
* is
* my
* multiline
* string""")
* 'Humpty ' + 'Dumpty'
* 'Ice ' * 2 + 'Baby'
* 5 + ' Fingers' #gives error
* str(5) + ' Fingers'
* '5' + 5 #gives error

#### 1.2 Math/Types
* 2 + 2
* 2 + 2 #this is a comment for humans to read
* 2.0 + 2
* 2 - 0
* 3 * 2
* 3 / 2
* 3 ** 2
* 9 // 2
* 9 % 2
* int('5') + 5
* float('2') + 2

#### 1.3 Variables
* x = 5
* x
* x = x + 1
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
* x = input()
* x

#### 1.4 Conditionals
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

#### 1.5 Loops
* for i in range(5):
  * print(i)
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

#### 1.6 Lists/Ranges
* my_list = []
* my_list
* my_list = [1,2,3,4,5]
* my_list[0]
* my_list[2]
* 4 in my_list
* len(my_list)
* my_list.append(10)
* my_list
* my_list.insert(3,8)
* my_list
* my_list.index(8)
* my_list.index(10)
* my_list.remove(8)
* range(7)
* list(range(7))
* list(range(2,9))
* list(range(2,19,3))

#### 2.0 Functions
* def my_function():
  * print('This is my function')
* my_function()
* def my_function():
  * return 5
* 3 + my_function()
* def my_function():
  * return 5
  * print('This is my function') # not printed because it's after the return statement
* 3 + my_function()

#### 2.1 Modules
* import random
* random.randint(1,100)
* from random import randint
* randint(1,100)
* from random import * # imports all objects in the module and removes the need for 'random.'
* x = list(range(10))
* shuffle(x) # this is a function from the module random

#### 2.2 Exceptions
* try:
  * x = int(input('Enter a number: '))
* except:
  * print('Invalid input')
* else:
  * print('Entered ' + x)
* x = 5
* assert x < 4, 'x is not less than 4'

#### 2.3 File Manipulation
* with open('my_file.txt','w') as f:
  * f.write('my text to write to file') # check the directory you were in when you started python for the my_file.txt you just created 
* with open('my_file.txt','w') as f:
  * f.write('this is more text to write') # the new text overwrote the old text
* with open('my_file.txt','a') as f: # the 'a' will let us add on to the old text instead of overwriting
  * f.write('\nI am now adding new text')
* with open('my_file.txt') as f:
  * cont = f.read()
* print(cont)
* with open('my_file.txt') as f:
  * cont = f.readlines()
* print(cont)

#### 2.4 Dictionaries/Tuples/Slices
* x = {'Name': 'Stitch', 'Species': 'Monster'}
* x['Name']
* 'Species' in x
* 'Monster' in x # false, because 'in' only checks keys and not values
* x = 1,2,3,4,5,6,7,8
* x
* x[3:7]
* x[:5]
* x[2:]
* x[::-1]

#### 2.5 chr()/ord()/.split()/.format()
* for i in range(65,90):
  * print(chr(i))
* for i in 'abcdefgh':
  * print(ord(i))
* x = 'this is sparta'
* x.split(' ')
* x
* '{} cuts deeper than {}'.format('fear','swords')

#### _here are some interesting leads that these exercises do not cover_

* standard libraries other than random
* regular expressions

##### to be added on

* .isalpha()
* .translate()
* lambda x: x**2
* map(function, iterable)
* filter(function, iterable)
* yield
* set()
* .add
* .remove
* .pop
* '.'
* '..'
* if __name__ == '__main__':
* #!/usr/bin/python
* '''…'''
* __attribute
* def func(self):
* def __init__(self):
* (?P<name>...)
* (?:...)
* |
* class subc(class):
* def __add__(self,other):
* .format
* @classmethod
* @property
* @myproperty.setter
* @myproperty.deleter
* *args
* **kwargs
