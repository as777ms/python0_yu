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

# 🧑‍🤝‍🧑 Lists
```bash
friends = ["Tom", "Henry", "Andrey"]
print(friends[0])
```

#
#
#
#
#

### 🧠 Final Notes
#### These are raw notes, taken directly while watching the tutorial

#### Every explanation and comment reflects how I personally understood the topic

#### Not meant to be perfect — just real, practical progress 💪


