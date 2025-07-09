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


```bash
is_male = False

if is_male:
     print("You are male")
else:
     print("You are female")
```
#
#
#
#

```bash
is_male = True
is_tall = False
if is_male and is_tall:
     print("You are tall male")
elif is_male and not(is_tall):
     print("You are a short male")
elif not(is_male) and is_tall:
     print("You are not a male but tall")
else:
     print("You are not a male but not tall")
```


#
#
#
#
#


# IF STATEMENTS & COMPARISONS

```bash
def max_num(num1, num2, num3):
    if num1 >num2 and num1 >num3:
        return num1
    elif num2 > num1 and num2 > num3:
        return num2
    else:
        return num3

print(max_num(4, 2,3))
```

#
#
#

### trying to build a calculator

```bash
num1 = float(input("Enter first Number: "))
op = input("Enter operator: ")
num2 = float(input("Enter second Number: "))

if op == "+":
    print (num1 + num2)
elif op == "-":
    print (num1 - num2)
elif op == "/":
    print(num1 // num2)
elif op == "*":
    print(num1 * num2)
else:
    print("Invalid Operator")
```

#
#
#
#
#
#


# DICTIONARIES

### key walues per

### when we want to acces to some information inside this key we can acces by using its key


### first we give it specific name example
```python
monthConversions = {
    "Jan": "January",
    "Feb": "February",
    "Mar": "March",
    "Apr": "April",
    "May": "May",
    "Jun": "June",
    "Jul": "July",
    "Aug": "August",
    "Sep": "September",
    "Oct": "October",
    "Nov": "November",
    "Dec": "December"
    # KEY : WALLUE
    # as a KEY we can use number too
}
# ! WARRNING keys must be uniq


# first way
print(monthConversions["Nov"])

# second way
print(monthConversions.get("Jan", "Not a valid key"))
```


#
#
#
#
#
#
#

# WHILE

```bash
i = 1
while i<=10:
    # as long as this guy (i<=10) is True we gonna loop through this i += 1 we gonna add 1 to i
    # now we gonna do , wo gonna go again to this while declaration and check that again until its True
    #  on every iteration throuth the loop and this point i is equel to 2 bcs it truns arround for the last time and this will repeat 10 time
    #  till its getting True and stops the loop ( in general as long we are not true we are keep executing through our loop)
    print(i)
    # i = i + 1
    i += 1

print("Done with loop")
```

#
#
#
#
#

```bash
i = 1
while i<=10:
    # as long as this guy (i<=10) is True we gonna loop through this i += 1 we gonna add 1 to i
    # now we gonna do , wo gonna go again to this while declaration and check that again until its True
    #  on every iteration throuth the loop and this point i is equel to 2 bcs it truns arround for the last time and this will repeat 10 time
    #  till its getting True and stops the loop ( in general as long we are not true we are keep executing through our loop)
    print(i)
    # i = i + 1
    i += 1

print("Done with loop")
```



#
#
#
#
#
#
#




# Building A Guessing Game

### here we gona use if statements, while loop and vars, and all that cool things to specify sicret word and user must interact with program
### user must be able to keep guessing what is the secret word is and keep typing in different responses untill they get the secret word
### now lets go had and create it
#
#
#
#
#
```bash
# secret word
secret_word = "giraffe"
# varieble to store users guess
guess = ""


# if they dont guess it correctly we want them to promt it correctly again
# so we cant just use a single input statement
# we actually have to use something called while loop and we can use the while loop in order to continuenly ask the person
    # to guess the word untill they guess it correctly

    # so lets go head and create a while loop
    # after creating while we need to specify a looping condition or a looping guard
    # it means as long as its true we gonna keep looping through this loop so basicly we wanna say we gonna keep looping
    # as long as users guess is not equel to the secret word
while guess != secret_word:

# so we gonna here ask them to input secret word
# here we can take this guess varieble and set it equel to input
    guess = input("Enter a guess: ")
    # we are storring watever user prints inside this guess = "" varieble

print("You win!")
```
#
#
#
#

## full code down here without explanation
#
```bash
secret_word = "giraffe"
guess = ""

while guess != secret_word:
    guess = input("Enter guess: ")

print("You win! ")
```

__________________________________________________________

### so right now we gonna set limit to it
### limmit of 3 tries if they win win if not lose the game



```bash
secret_word = "giraffe"
guess = ""
# under here we gonna create a cnt of how many times does user has got tiket to find a guees
guess_count = 0
# here we gonna create another element that called guess limit
guess_limit = 3
# here is one another var to stop loop if it is False it means user is still in game id True it means Nah game over buddy
out_of_guess = False
while guess != secret_word and not(out_of_guess):
    # top and if their not out of 👆 guesses then we gonna keep looping
    # we come here after limits var creating
    # first in the top we must to check does person end up with his tikets or no
    if guess_count < guess_limit:
        guess = input("Enter guess: ")
        # down here after writing guess_count (every time we go throught the loop we want to increment that guess count
        guess_count += 1
    else:
        out_of_guess = True

# and if the user as we set in the top oout of guesses if its true we print your out
if out_of_guess:
    print("You LOSE! buddy ")
    # if they not out of guesses that means that they guess the word cocrrectly
else:
    print("You win! ")
```

#
#
#
#
#
#
#


# For loop

# for

### it allows us to loop over different collections of items arrays, letters inside str, numbers....

```bash
for letter in "Giraffe Academy":
    # its gonna say (for) every (letter) inside this "Giraffe Academy"
    print(letter)
    # so how it works we can define the varieble and that varieble will change on each ideration of the loop
    # so in the first ideartion of the loop this (letter) varieble represented a "G" letter on the seccond ideration of the loop "i"
```
#
#

### here we can use it in array

```bash
friends = ["Tom", "Gaga", "Charli", "Troye"]

for friend in friends:
    print(friend)
```


#
#
#
#
### here it is about numbers

```bash
num1 = 10

for index in range(num1 +1 ):
    print(index)
```

#
#
#
```bash
num1 = 10
for index in range(1, num1 +1 ):
    print(index)
```
#
#
#

```bash
for index in range(10):
    print(index)
```
#
#
#
```bash
for index in range(3, 10):
    print(index)
```

##
#
#
#
#

```bash
friends = ["Tom", "Gaga", "Charli", "Troye"]

for friend in range(len(friends)):
    # print(friend)
    # print(friends[friend])
    print(friends[0])
```

#
#
#
#



```bash
for index in range(5):
    if index == 0:
        print("first Iteration")
    else:
        print("not a first Iteration")
```





# EXPONENT FUNCTION
###  2^3 it  calls 2 raised to the 3 power
#
#
#

```bash
def raise_to_power(base_num, power_num):
    # so wegonna take the base_num and power it to power_num
    # so right now we dont know which walue can user add in power_num bcs we need qube only so bcs of it we agoing to create a for
    result = 1
    for index in range(power_num):
        # it means we loop sroth it as many as power_num
        # result *= base_num
    # or
        result = result * base_num
    return result

print(raise_to_power(2, 3))
```




#
#
#
#
#
#



# 2D list & Nested Loops

```bash
number_grid = [
    [1,2,3],
    [4,5,6],
    [7,8,9],
    [0]
]

print(number_grid[2][1])

#nested for loop


for row in number_grid:
    # print(row) we need to create another for loop to acces inside its
    for column in row:
        print(column)
```
#
#
#
#
#



# Build a translator


### the rule is any vowel becomes a g
```bash
def translate(phrase):
    translation = ' '
    for letter in phrase:
        if letter in "AEIOUaeiou":
            if letter.isupper():
                translation = translation + "G"
            else:
            # it means if the letter inside this string is that aeiou it checks that...
                translation = translation + "g"
        else:
            translation = translation + letter
    return translation

print(translate(input("Enter a phrase: ")))
```


#
#
#
#
#

# Commnets

