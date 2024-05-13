# PYTHON String Manipulation

In this playground we will write introduce 5 programs that will convert a string into Title Case, PascalCase, snake_case, camelCase and Kebab-Case.

Here are some of the Python built-in functions we will be using:
1. ```.title()```
2. ```.lower()```
3. ```.replace()```
4. ```.split()```
5. ```.join()```



## Program 1: "Title Case"
This is the simplest case to implement. Title Case is written where the first letter of each word is capitalised.
Luckily, Python has a built in function for this:
```python runnable
string = "this is a string."

print(string.title())
```
The result of this code will be: "This Is A String."

## Program 2: "PascalCase"
PascalCase is when the string is written with the first letter of each word being capitalised, and then with all the spaces in the string being removed.
We will define our own function which uses ```.title()```:
```python runnable
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
```python runnable
string = "this is a string."

def snake_case(string):
    string = string.lower()
    string = string.replace(" ","_")
    return string
```
The result of this code will be: "this_is_a_string."

## Program 4: "camelCase"
When we implement camelCase, you might notice that it is similar to "PascalCase". The code is similar, but we leave the first letter of the first word in lowercase.
We will define our own function for this:
```python runnable
string = "this is a string."

def camelCase(string):
    return "".join(t.title() for t in s.split())
```
The result of this code will be: "thisIsAString."

## Program 5: "kebab-case"
Similar to snake_case, we can also write strings in kebab-case... the only exception is that instead of using underscores to replace spaces, we use hyphens.
We will define our own function for this:
```python runnable
string = "this is a string."

def kebab_case(string):
    string = string.lower()
    string = string.replace(" ","-")
    return string
```
The result of this code will be "this-is-a-string."

### Conclusion
In this tutorial we have created 5 programs to manipulate string into "Title Case", "PascalCase", "snake_case", "camelCase" and "kebab-case".

Here are some links to learn more of the built-in functions we mentioned previously:
https://www.w3schools.com/python/ref_string_title.asp

https://www.w3schools.com/python/ref_string_lower.asp

https://www.w3schools.com/python/ref_string_replace.asp

https://www.w3schools.com/python/ref_string_split.asp

https://www.w3schools.com/python/ref_string_join.asp

Please feel free to use this code in your clashes or programs.

Happy Coding,
@Code-Parser