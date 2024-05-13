# PYTHON String Manipulation

In this playground we will write introduce 5 programs that will convert a string into Title Case, PascalCase, snake_case, camelCase and Kebab-Case.

## Program 1: "Title Case"
This is the simplest case to implement. Title Case is written where the first letter of each word is capitalised.
Luckily, Python has a built in function for this:
```
string = "this is a string."

print(string.title())
```
The result of this code will be: "This Is A String."

## Program 2: "PascalCase"
PascalCase is when the string is written with the first letter of each word being capitalised, and then with all the spaces in the string being removed.
We will define our own function which uses ```.title()```:
```
string = "this is a string."

def PascalCase(string):
    string = string.title()
    string = string.replace(" ","")
    return string
```
The result of this code will be: "ThisIsAString."

## Program 3: "snake_case"
We simply convert the entire string to lowercase and then replace each space with an underscore.
We will define our own function for this:
```
string = "this is a string."

def snake_case(string):
    string = string.lower()
    string = string.replace(" ","_")
    return string
```
The result of this code will be: "this_is_a_string."