# 🐍 Python Beginner Notes — Based on freeCodeCamp YT Course

## 👤 Variables and Strings

```python
character_name = "Tom"
character_age = "17"

print("There was a man with a name of " + character_name + ", ")
print("he was "+ character_age + ", "+ "years old")

character_name = "Any"
print("he really liked the name" ", " + character_name)
print("but didn't like being " + character_age)
```


```
print("Giraffe Academy")
print("Giraffe\nAcademy")
```

we need this backslesh to pronounce quetetion mark not new line bcs if we do it in this way print("Giraffe"Academy") it will end "Giraffe" like this and start new string
```bash
print("Giraffe\"Academy")
```


#
#
#
#
#

# 🔡 String Methods


### Hurrey im learning pythons string methods
```bash
phrase = "Giraffe Academy"
print(phrase.lower())
print(phrase.upper())
```

#### here we can check does string entairly lowercase or uppercase
```bash
print(phrase.isupper())
```


#### now we can use them in combinations together with each other

```bash
print(phrase.upper().islower())
print(phrase.upper().isupper())
```


#### now we can see the lens of the string (how many characters does exist there )
```bash
print(len(phrase))
```

#### here we can grab individual characters inside of our string by using their index started from 0

```bash
print(phrase[0])
```

#### getting index of string in python (we give it parametr not value )
```bash
print(phrase.index("G"))
``` 

#### replace function first parrametr is what im going to replace and second is whith what am i going to replace it
```bash
print(phrase.replace("Giraffe", "Elephant"))
```





_____




# Working with numbers in python Numbers are the most common in python codding
## mathematical opeartions and funcitons
```bash
print(2)
```

#### converting number into a string
#### it helps us print out our numbers along our string  bcs if we are not converting number to string while conceting num and string it gives TypeError
```bash
my_num = 7
print(str(my_num) + " 1is my favourite number")
```

#### abs function gives absolute value of varaeble (it gives us absolute value of negative 7)
```bash
num = -7
print(abs(num))
```

#### pow function daraja it gives power to that number and it takes 2  it allow to us path there 2 piece of information 1. is number and the 2. is the power that we want to take to that number too
#### it just works ;ike this 3^2 (it just wanna be 3 rased to the power of 2)
```bash
print(pow(3, 2))
```

#### max it checks and tell us which number is higher
```bash
print(max(3,4,5))
```

#### min it checks and tell us which number is smaller
```bash
print(min(2,3,4,4,1,-4))
```

#### round function to round numbers
```bash
print(round(3.2))
```
#### but if i say 3.7 it gonna round it to 4
```bash
print(round(3.7))
```

________
#
#
#
#
#
#


#

> [!TIP] 🧠 Math Module Functions

```bash
from math import *
```
#### another function that we couldnt work without this import is floor function it just greb the lower numbers not like round
```bash
print(floor(3.7))
```
#### here in ceil no matter if it is 3.1 upper well get 4
```bash
print(ceil(3.1))
```
#### sqrt this chould gonna return  to us sqr root number
```bash
print(sqrt(36))
```


#
#
#
#
#
#
#
#

> [!NOTE]👂 Getting User Input


```bash
name = input("Enter your name ")
age = input("Enter your age ")
print("Hello, dear " + name + " !\n" "You are " + age)
```

# Simple Calculator
```bash
num1 = input("Enter a number: ")
num2 = input("Enter another number: ")
result = int(num1) + int(num2)
# result2 = float(num1) + float(num2)

print(result)
```


> [!TIP] 🎮 Mad Libs Game

```bash
color = input("Enter a color: ")
plural_noun = input("Enter a plural noun: ")
celebrity = input("Enter a celebrity: ")

print("Roses are " + color)
print(plural_noun + " are blue")
print("I love " + celebrity)
```
#### Home Task to do that again

#
#
#
#
#
#
#


#
#
#
#
#

### 🧠 Final Notes
#### These are raw notes, taken directly while watching the tutorial

#### Every explanation and comment reflects how I personally understood the topic

#### Not meant to be perfect — just real, practical progress 💪

# # # # # # # # # # # # #  #
#
#
#
#
#

# 🧑‍🤝‍🧑 Lists
```bash
friends = ["Tom", "Henry", "Andrey"]
print(friends[0])
```

```bash
lucky_numbers = [4, 5, 3, 8, 21, 7]
friends = ["Tom", "Henry", "Andrey","Andrey", "Adele", "Gaga"]
```
### here is the function that helps us to extend one list to another it adds another lists ellemend in the end to the existed list
```bash
friends.extend(lucky_numbers)
```
### we can too add individuel ellements onto a list it can help append another item onto the end of the list (addds to the end)
```bash
friends.append("Jim")
```

### another function that can help to us to add item in the middle of the list it takes 2 parametrs
```bash
friends.insert(1, "Alem")
```
### removing elements it works by typing the name of the item not its index
```bash
friends.remove("Henry")
```
### this function can remove the entire list and give us empty list
```bash
friends.clear()
```

### this function pop off removes last item of the list
```bash
friends.pop()
```
### here is another function that helps us to check gives us its index if the item doesnt exist in the list it gives error in console
```bash
print(friends.index("Henry"))
```

### here we have got function that counts how many times does item was in the list (it counts the same items)
```bash
print(friends.count("Andrey"))
```
### also we have got sort function that sorts intems into alphabetical order
```bash
friends.sort()
```
### we can also reverse the list
```bash
lucky_numbers.reverse()
print(lucky_numbers)
```
### another function that copies lists items
```bash
friends2 = friends.copy()
print(friends2)
print(friends)
```


#
#
#
#
##
#
#


# Tuples




```bash
coordinates = (4, 5)
```
### here we can equel one coordinate by using its index to something else it would give to us error that (TypeError: 'tuple' object does not support item assignment)
#### in tuples we cant mutate our tuple we cant eddit delet or do some stuuf like we done with the list
#### we use tuples in practise for data that we never gonna change data cant me mutadet
```bash
coordinates[1] = 10
```
#### here we can create a list of tuples
```bash
coordinates = [(4, 5), (6, 7), (80, 34)]
```
#### SO THE REAL TRUTH IS THAT WE USE TUPLES WHEN WE DONT WANT TO CHANGE DATA MUTADE IT ITS LIKE CONST IN JS A LITTLE SO IN REAL WORK WE SHOULD WORK ONLY BY USING LIST

```bash
print(coordinates[1])
```
_______________________
#
#
#
#
#
#
#
#




# Functions

### in python when python sees (def) it understands that person wants to use function and calls it

```bash
def say_hi():
     print("Hello User")
say_hi()
```
### after creating def we are givint it a name ;like giving a name to a varieble and yep any code inside the function
### must be intended and if it writes out of that function it is out of the function



```bash
def say_hi():
     print("Hello User")


print("Top")
say_hi()
print("Bottom")
```
### here in top i think there is no explanation needs bcs first first it intead the code out of function after into of it after in the end as you see
#
#

### another thing we can do with functions is like adding parametr into it

```bash
def say_hi(name):
     print("Hello", name)

say_hi("Anisa")
say_hi("Andrey")
```
### we can also include it more than one parametrs
#
#
```bash
def say_hi(name, age):
    print("Hello", name)
    print("You are " + age + " years old")
say_hi("Anisa", "17")
```

#
#
#
#
#
#
#
#
#
#
#


# Return statement

#### return gives a walue wathewer it calls a function it allows us to return whats a calling function

```bash
def cube(num):
    return num ** 3
print(cube(4))
```
#
#
#
### here is another way of returnning this kind of function

```bash
def cube(num):
    return num * num * num
     # print("code")
result = cube(4)
print(result)
```

### and yep WARNING we are not able to put any code after return statement

#
#
#
#
#
#
#
#
#


# If statement

### we are giving to it condition and it will give to us true or false if its true we return true one
