Lecture 4: Variables and Data Types
Author Name : Shaista Adnan

Linkedin : linkedin.com/in/iamahsanalirajpoot
Facebook : facebook.com/iamahsanalirajpoot
GitHub : github.com/iamahsanalirajpoot
Kaggle : kaggle.com/ahsanalirajpoot
Variables In Python
What Are Variables?
A variable is a container that temporarily stores data during the execution of a program.
The value stored in a variable can change during the program's execution, which is why it is called a "variable."
Rules for Naming Variables:
Key Rules:

Start with a Letter or Underscore: Variable names must begin with a letter (a-z, A-Z) or an underscore (_).
Example: username, _firstname

Cannot start with a Number: Variable names cannot begin with a digit.
Example: 1user is invalid, but user1 is valid.

Use Only Letters, Numbers, and Underscores: Variable names can only contain letters, numbers, and underscores.
Example: user_name, age1

Case-Sensitive: Variable names are case-sensitive.
Example: FirstName and firstname are considered two different variables.

Avoid Reserved Words: Do not use Python’s reserved keywords (e.g., print, if, for) as variable names.
Example: print = 10 is invalid because print is a reserved word.

Meaningful Names: Use meaningful and descriptive names for variables to improve code readability.
Example: Use student_name instead of sn.

Initializing Variables
Syntax: To create a variable, you need three things:

Variable Name: The name of the variable (e.g., name).
Assignment Operator: The equal sign (=) is used to assign a value to the variable.
Value: The data you want to store in the variable (e.g., Ahsan).
Example:

Assigning a string value to a variable:

name = "Shaista"  # -> Here, 'name' is the variable name, and "Shaista" is the value assigned to it
Assigning an integer value to a variable:

age = 18  # -> Here, 'age' is the variable name, and "18" is the value assigned to it
Data Types in Python
What is Datatype
A data type is a classification that specifies the type of data a variable can hold. In Python, the main data types are:

Numeric Types: These include integers (int), floating-point numbers (float), and complex numbers (complex).

Text Type: This includes strings (str).

Sequence Types: These include lists (list), and tuples (tuple).

Mapping Type: This includes dictionaries (dict).

Set Types: These include sets (set) and frozensets (frozenset).

Boolean Type: This includes boolean values (bool), which can be either True or False.

None Type: This includes the NoneType, which has a single value, None.

1. Numeric Data Types
Numeric data types represent numbers and can be used for mathematical operations.

Integer (int)
Represents whole numbers, both positive and negative.
Example:

age = 26

print(type(age))  # -> type function will return type of data stored in variable
<class 'int'>
Float (float)
Represents real numbers with decimal points.
Example:

percentage_marks = 96.98
net_profit = -434.67

print(type(percentage_marks))
print(type(net_profit))
<class 'float'>
<class 'float'>
Represents numbers with a real and imaginary part.
Example:

complex_number = 4 + 6j

print(type(complex_number))
<class 'complex'>
2. Text Data Type
String (str)
Represents a sequence of characters enclosed in single or double quotes.
name = "Shaista"
full_name = 'Shaista Adnan'

print(type(name))
print(type(full_name))
<class 'str'>
<class 'str'>
Multiline strings:
Multiline strings can be created using triple quotes

# creating meaningful multiline string

multiline_str = """
Life is full of surprises,
Sometimes sunshine, sometimes rain.
Code runs perfectly at night,
But crashes during the day again.

Tea fuels the dreamers,
Errors teach us to grow.
Keep learning, keep building,
That's the developer's flow.
"""

print(type(multiline_str))
<class 'str'>
String Operations:
Concatenation: Joining two or more strings together using the + operator.

# string oncatenation
first_name = "Shaista"
last_name = "Adnan"
full_name = first_name + " " + last_name

print(full_name)
Shaista Adnan
Repetition: Repeating a string multiple times using the * operator.

# string repetition
laugh = "ha" * 5
print(laugh)
hahahahaha
Indexing: Accessing individual characters in a string using square brackets [] and passing the index of the character.

# string indexing
name = "Shaista Adnan"
first_char = name[0]  # -> 'A'
third_char = name[2]  # -> 's'

print(first_char)
print(third_char)
S
a
String Slicing:
Extracting a substring from a string using the colon : operator within square brackets [] and specifying the start and end indices.

# string slicing
name = "Shaista Adnan"
first_name = name[0:5]  # -> end index is exclusive and start index is inclusive
mid_name = name[6:9]
lst_name = name[10:18]

print(first_name)  # -> 'Shaista'
print(lst_name)    # -> 'Adnan'
Shaista
Adnan
f-string:
A way to format strings in Python by adding expressions/variables inside curly braces {} within a string prefixed with f.

name = "Shaista"
age = 26

# creating f-string
greeting = f"Hello, my name is {name} and I am {age} years old."

print(greeting)
Hello, my name is Shaista and I am 26 years old.
3. Sequence Types
Sequence types are ordered collections of items.
Before Jumping into the Sequence Types, let's understand the following concepts:

What is meant by Ordered?

Ordered means that the items in the sequence have a defined order, and you can access them using their index.
What is difference between mutable and immutable?

Mutable: Can be changed after creation (e.g., lists).
Immutable: Cannot be changed after creation (e.g., tuples, strings).
List
Represents an ordered, mutable collection of items.
Creating a List:
We use square brackets [] to create a list

list_of_numbers = [1, 3, 5, 6, 7, 8, 9, 10]

print(list_of_numbers)
print(type(list_of_numbers))
[1, 3, 5, 6, 7, 8, 9, 10]
<class 'list'>
# Creating a list with mixed data types
mixed_list = [1, "Junaid", 3.14, True, None]

print(mixed_list)
[1, 'Junaid', 3.14, True, None]
Accessing List Elements:
We can access the list element by their index number, Each element in a list has an index, starting from 0

list_of_numbers = [1, 2, 3, 4, 5]

print(list_of_numbers[0])  # -> Accessing the first element of the list
print(list_of_numbers[1])  # -> Accessing the second element of the list
print(list_of_numbers[-1]) # -> Accessing the last element of the list
print(list_of_numbers[-2]) # -> Accessing the 2nd last element of the list
1
2
5
4
Slicing Lists:
We can extract a portion of the list using slicing, which allows us to specify a start and end index.

items = ["Apple", "Banana", "Orange", "Strawbarry", "Mango"]

print(items[2:5])  # -> Slicing the list to get elements from index 2 to 4 (5 is exclusive)
['Orange', 'Strawbarry', 'Mango']
Adding List Element:
Using append() (Adds one item to the end)
items = [10, 20, 30]
items.append(40)  # -> adds 40 at the end
print(items)
[10, 20, 30, 40]
Using insert(index, value) (Adds item at specific position)
items = [10, 30, 40]
items.insert(1, 20)  # -> inserts 20 at index 1
print(items)
[10, 20, 30, 40]
Using extend() (Adds multiple items from another list)
items = [2, 4, 6, 8]
items.extend([10, 12, 14])  # -> adds multiple elements

print(items)
[2, 4, 6, 8, 10, 12, 14]
Using + operator (Combines two lists (creates new list))
list_1 = [1, 2, 3]
list_2 = [4, 5, 6]
combined = list_1 + list_2  # -> new combined list
print(combined)
[1, 2, 3, 4, 5, 6]
Using *= n (Repeat list elements)
items = ['a', 'b', 'c']
items *= 3  # -> repeats list 3 times
print(items)
['a', 'b', 'c', 'a', 'b', 'c', 'a', 'b', 'c']
Removing List Elements:
Using pop() (removes last element)
items = [10, 20, 30, 40, 50]
items.pop()  # -> removes last element
print(items)
[10, 20, 30, 40]
Using pop(index) (removes specific index)
items = [10, 20, 30, 40, 50]
items.pop(1)  # -> removes element at index 1 (value = 20)
print(items)
[10, 30, 40, 50]
Using remove(value) (removes first occurrence)
items = [10, 20, 30, 20, 50]
items.remove(20)  # -> removes first occurrence of 20
print(items)
[10, 30, 20, 50]
Using del with index
items = [10, 20, 30, 40, 50]
del items[2]  # -> deletes item at index 2 (value = 30)
print(items)
[10, 20, 40, 50]
Using del with slice
items = [10, 20, 30, 40, 50]
del items[1:4]  # -> deletes from index 1 to 3 (20, 30, 40)
print(items)
[10, 50]
Using clear() to empty entire list
items = [10, 20, 30, 40, 50]
items.clear()  # -> clears all elements
print(items)
[]
List Sorting (with sort() and sorted()):
# using sort()
numbers = [4, 1, 3, 5, 2]
numbers.sort()  # -> modifies in place
print(numbers)  # [1, 2, 3, 4, 5]


# Descending order
numbers.sort(reverse=True)
print(numbers)  # [5, 4, 3, 2, 1]
[1, 2, 3, 4, 5]
[5, 4, 3, 2, 1]
# using sorted()
# sorted() returns new list
numbers = [4, 1, 3, 5, 2]
sorted_list = sorted(numbers)

print(sorted_list)
[1, 2, 3, 4, 5]
Min & Max in a List:
min(): Returns the smallest item in the list.
max(): Returns the largest item in the list.
numbers = [10, 45, 3, 99, 24]

print(min(numbers))  #  3
print(max(numbers))  #  99
3
99
Looping Through List:
Basic for Loop
fruits = ["apple", "banana", "mango"]

for fruit in fruits:
    print(fruit)
apple
banana
mango
Using enumerate() (Index + Value)
for index, fruit in enumerate(fruits):
    print(f"{index}: {fruit}")
0: apple
1: banana
2: mango
Nested Lists:
nested_lists = [[1, 2], [3, 4], [5, 6]]
print(nested_lists)
[[1, 2], [3, 4], [5, 6]]
Membership Test: in and not in:
fruits = ["apple", "banana"]
print("apple" in fruits)      # True
print("mango" in fruits)      # False
print("mango" not in fruits)  # True
print("apple" not in fruits)  # False
True
False
True
False
Converting from Other Types into List:
# String to list
num_str = "123456"
num_list = list(num_str)
print(num_list)
['1', '2', '3', '4', '5', '6']
# Tuple to list
num_tuple = (1, 2, 3)
num_list = list(num_tuple)
print(num_list)
[1, 2, 3]
# Split string into list
text = "life is not easy"
words = text.split()
print(words)
['life', 'is', 'not', 'easy']
List Comprehensions:
squares = [x**2 for x in range(1, 6)]
print(squares)
[1, 4, 9, 16, 25]
Tuple
An ordered collection of elements, similar to a list, but immutable (cannot be changed).
Creating a Tuple:
We use round brackets () to create a tuple

tuple_of_num = (1, 2, 3, 4, 5)

print(tuple_of_num)
print(type(tuple_of_num))
(1, 2, 3, 4, 5)
<class 'tuple'>
# Creating a tuple with mixed data types
mixed_tuple = (1, "Hassan", 3.14, True, None)
print(mixed_tuple)
(1, 'Hassan', 3.14, True, None)
Accessing Tuple Elements:
We can access the tuple element by their index number, Each element in a tuple has an index, starting from 0

tuple_of_num = (1, 2, 3, 4, 5)

print(tuple_of_num[0])  #-> accessing first element
print(tuple_of_num[1])  #-> accessing second element
print(tuple_of_num[-1]) #-> accessing last element
print(tuple_of_num[-2]) #-> accessing second last element
1
2
5
4
Slicing Tuples:
We can extract a portion of the tuple using slicing, which allows us to specify a start and end index.

num_tuple = (1, 2, 3, 4, 5)
first_two = num_tuple[0:2]  # -> slicing to get first two elements
print(first_two)
(1, 2)
Adding Tuple Elements:
Tuples are immutable, meaning you cannot add or change elements once the tuple is created. However, you can create a new tuple that includes the elements of the original tuple plus the new elements.

Using + Operator (Concatenation)
# Creates a new tuple by adding another tuple
t = (1, 2, 3)
t = t + (4,)  # Note the comma (,) to make it a tuple
print(t)
(1, 2, 3, 4)
# Adding Multiple Elements
t = (1, 2, 3)
t += (4, 5, 6)
print(t)
(1, 2, 3, 4, 5, 6)
Converting to List and Back to Tuple
t = (1, 2, 3)
temp = list(t)      # -> Convert to list
temp.append(4)      # -> Add element
t = tuple(temp)     # -> Convert back to tuple
print(t)
(1, 2, 3, 4)
Reminder:

Tuples are immutable, so each of these methods creates a new tuple.
Always include a comma when adding a single element: (6,) not (6)
Remove Tuple Elements:
Since tuples are immutable, you cannot remove elements from them directly. However, you can create a new tuple that excludes the elements you want to remove.

Convert Tuple to List, Remove, Then Back
t = (10, 20, 30, 40)
temp = list(t)
temp.remove(30)    # -> remove by value
t = tuple(temp)
print(t)
(10, 20, 40)
min & max in a Tuple:
min(): Returns the smallest item in the tuple.
max(): Returns the largest item in the tuple.
numbers = (-3, 34, 23, 67, 109, 4)

print(min(numbers)) # -3
print(max(numbers)) # 109
-3
109
Using Tuple Slicing and Concatenation
# removing 3 from tuple
t = (1, 2, 3, 4, 5)
t = t[:2] + t[3:]  # -> # Keep elements before index 2 and after index 2 (skip index 2)
print(t)
(1, 2, 4, 5)
Important Notes:

You cannot use remove() or pop() directly on a tuple.
These tricks create a new tuple each time.
Tuple unpacking:
Tuple unpacking allows you to assign the elements of a tuple to multiple variables in a single line.

person = ("Humza", 18, "Pakistan")
name, age, country = person  # -> Unpacking the tuple into variables

print(name)     # -> 'Humza'
print(age)      # -> 18
print(country)  # -> 'Pakistan'
Humza
18
Pakistan
# Using * to unpack
a, *b, c = (1, 2, 3, 4, 5)
print(a)  # -> 1
print(b)  # -> [2, 3, 4] (a list)
print(c)  # -> 5
1
[2, 3, 4]
5
Looping Through Tuples:
Basic for Loop
colors = ("red", "green", "blue")

for color in colors:
    print(color)
red
green
blue
Using enumerate()
for index, color in enumerate(colors):
    print(f"{index}: {color}")
0: red
1: green
2: blue
Nested Tuples:
Tuples can contain other tuples, allowing for complex data structures.

nested_t = ((1, 2), (3, 4))
print(nested_t)
((1, 2), (3, 4))
4. Mapping Type
Dictionary
Represents an unordered collection of key-value pairs.
Keys must be unique and immutable (e.g., strings, numbers, tuples).
Values can be of any data type and can be duplicated.
Creating a Dictionary:
We use curly braces {} to create a dictionary
# creating dictionary
person = {
    "name": "Ali",
    "age": 18,
    "country": "Pakistan"
}

print(person)
{'name': 'Ali', 'age': 18, 'country': 'Pakistan'}
creating a dictionary with keys and values
keys = ["name", "age", "location"]
values = ["Ali", 20, "Balakot"]

# Combining keys and values into a dictionary using zip()
person_dic = dict(zip(keys, values))

print(type(person_dic))
print(person_dic)
<class 'dict'>
{'name': 'Ali', 'age': 20, 'location': 'Balakot'}
Accessing Elements in a Dictionary:
Use square brackets [] with the key to access values
person = {
    "name": "Ali",
    "age": 18,
    "country": "Pakistan"
}

# Accessing values by keys
name = person["name"]
age = person["age"]
country = person["country"]

print(name)
print(age)
print(country)
Ali
18
Pakistan
Using .get() method is a best practice as it prevents exceptions
person = {
    "name": "Ali",
    "age": 18,
    "country": "Pakistan"
}

name = person.get("name")
age = person.get("age")

print(name)
print(age)
Ahsan
18
print(person.get("adress")) # -> None, .get() doesn't raise error if key is missing
None
Accessing All Keys, Values, and Items
student = {"name": "Ali", "age": 20, "course": "Data Science"}

student_keys = student.keys()
student_values = student.values()
student_items = student.items()

print(f"Student Keys : {student_keys}")
print(f"Student Values : {student_values}")
print(f"Student Items : {student_items}")
Student Keys : dict_keys(['name', 'age', 'course'])
Student Values : dict_values(['Ali', 20, 'Data Science'])
Student Items : dict_items([('name', 'Ahsan'), ('age', 20), ('course', 'Data Science')])
Adding New Elements in Dictionary:
student = {"name": "Ali", "age": 18}

# Adding new elements
student["course"] = "AI"
student["grade"] = "A"

print(student)
{'name': 'Ali', 'age': 18, 'course': 'AI', 'grade': 'A'}
You can even add a list or tuple as a value
student["hobbies"] = ["reading", "coding", "cricket"]

print(student)
{'name': 'Ali', 'age': 18, 'course': 'AI', 'grade': 'A', 'hobbies': ['reading', 'coding', 'cricket']}
Updating Values in a Dictionary:
To update a value, just assign a new value to an existing key

student = {"name": "Ali", "age": 20, "course": "AI"}
print(f"Before updating: {student}")

# Updating existing values
student["age"] = 18                 # -> Updates age
student["course"] = "Data Science"  # -> Updates course

print(f"After updating: {student}")
Before updating: {'name': 'Ali', 'age': 20, 'course': 'AI'}
After updating: {'name': 'Ali', 'age': 18, 'course': 'Data Science'}
Using .update() Method
-> .update() is useful for updating multiple key-value pairs at once.
-> If the key exists, it updates. If not, it adds it (acts like add + update).

student = {"name" : "Ahsan", "age" : 18, "grade" : "A"}
print(f"Before updating: {student}")

# updating name and grade
student.update({"name": "Ahsan Ali", "grade": "A+"})
print(f"After updating: {student}")
Before updating: {'name': 'Anum', 'age': 18, 'grade': 'A'}
After updating: {'name': 'Anum Ali', 'age': 18, 'grade': 'A+'}
Deleting Elements from a Dictionary:
del Keyword: Deletes a key-value pair by key
student = {"name": "Anum", "age": 20, "course": "AI"}
del student["age"]  # Removes 'age' key
print(student)
{'name': 'Ahsan', 'course': 'AI'}
.pop(key) Removes the key-value pair and returns the value.
student = {"name": "Anjum", "age": 20, "course": "AI"}
removed_value = student.pop("course")  # Removes 'course' and stores its value
print(student)
print("Removed:", removed_value)
{'name': 'Anjum', 'age': 20}
Removed: AI
.popitem() Removes last inserted item
student = {"name": "Anjum", "age": 20, "course": "AI"}
student.popitem()
print(student)
{'name': 'Anjum', 'age': 20}
.clear() Removes all items

student = {"name": "Anjum", "age": 20, "course": "AI"}
student.clear()
print(student)
{}
Looping Through a Dictionary:
Loop Through Keys
student = {"name": "Anjum", "age": 20, "course": "AI"}

for key in student:
    print(key)
name
age
course
Loop Through Values
for value in student.values():
    print(value)
Ahsan
20
AI
Loop Through Key-Value Pairs
for key, value in student.items():
    print(f"{key} → {value}")
name → Anjum
age → 20
course → AI
Using enumerate() to get index and value
for index, (key, value) in enumerate(student.items()):
    print(f"{index}. {key} → {value}")
0. name → Anjum
1. age → 20
2. course → AI
Nested Dictionaries:
A nested dictionary is a dictionary inside another dictionary, useful for representing complex structured data.

students = {
    "student1": {"name": "Anaya", "age": 18, "course": "AI"},
    "student2": {"name": "Shafiq", "age": 21, "course": "DS"}
}

print(students)
{'student1': {'name': 'Anaya', 'age': 18, 'course': 'AI'}, 'student2': {'name': 'Usman', 'age': 21, 'course': 'DS'}}
Accessing Nested Dictionary Values
# Accessing full inner dictionary
print(students['student1'])
{'name': 'Anaya', 'age': 18, 'course': 'AI'}
# Accessing a specific value inside inner dictionary
print(students["student1"]["name"])  # → Ahsan
print(students["student1"]["course"])  # → AI
Ahsan
AI
Adding New Inner Dictionary
students["student3"] = {"name": "Sara", "age": 21, "course": "ML"}
print(students)
{'student1': {'name': 'Anaya', 'age': 18, 'course': 'AI'}, 'student2': {'name': 'Shafiq', 'age': 21, 'course': 'DS'}, 'student3': {'name': 'Sara', 'age': 21, 'course': 'ML'}}
Updating Inner Values
students["student2"]["age"] = 23
Looping Through Nested Dictionary
print(students)
{'student1': {'name': 'Anaya', 'age': 18, 'course': 'AI'}, 'student2': {'name': 'Shafiq', 'age': 23, 'course': 'DS'}, 'student3': {'name': 'Sara', 'age': 21, 'course': 'ML'}}
for student, info in students.items():
    print("All students info:")
    print(f"\n{student} info:")
    for key, value in info.items():
        print(f"{key} → {value}")
All students info:

student1 info:
name → Anaya
age → 18
course → AI
All students info:

student2 info:
name → Shafiq
age → 23
course → DS
All students info:

student3 info:
name → Sara
age → 21
course → ML
5. Set Types
Set
A set is an unordered collection of unique elements.
Sets are mutable, meaning you can add or remove elements.
Created using curly braces {} or the set() function.
Creating a Set:
Using curly braces {}
num_set = {1, 2, 3, 4, 5}
print(type(num_set))
print(num_set)
<class 'set'>
{1, 2, 3, 4, 5}
Using set() Constructor
new_set = set([1, 2, 3, 4])  # from a list
print(new_set)
{1, 2, 3, 4}
word_set = set("shaista")  # from string → duplicates removed
print(word_set)
{'n', 'a', 's', 'h'}
mix_set = set((10, 20, 10, 30))  # from tuple
print(mix_set)
{10, 20, 30}
# empty set
empty_set = set()
print(empty_set)
print(type(empty_set))
set()
<class 'set'>
Set with Mixed Data Types
mix_set = {"AI", 101, 3.14, True}
print(mix_set)
{'AI', True, 3.14, 101}
Duplicate Values Are Removed Automatically
dup_set = {1, 2, 2, 3, 4, 4, 5, 5, 5}
print(dup_set)
{1, 2, 3, 4, 5}
Adding Set Elements:
Using add() (Add a single element) (Duplicates will be ignored)
my_set = {1, 2, 3}
my_set.add(4)  # adds 4 to the set
print(my_set)
{1, 2, 3, 4}
update() (Add multiple elements from an iterable)
my_set = {1, 2, 3}
my_set.update([4, 5, 6])  # adds all from the list
print(my_set)
{1, 2, 3, 4, 5, 6}
Removing Set Elements:
remove(): Removes a specific element, but throws an error if not found
my_set = {10, 20, 30}
my_set.remove(20)  # removes 20
print(my_set)

# my_set.remove(99)  ->  KeyError as 99 not in set
{10, 30}
discard(): Also removes a specific element, but no error if it doesn’t exist.
my_set = {1, 2, 3}
my_set.discard(2)  # removes 2
my_set.discard(99)  # no error
print(my_set)
{1, 3}
pop(): Removes random element and returns.
my_set = {5, 10, 15}
removed = my_set.pop()
print("Removed:", removed)
print(my_set)
Removed: 10
{5, 15}
clear(): Removes all elements (empties the set).
my_set = {1, 2, 3}
my_set.clear()
print(my_set)
set()
del: Deletes the entire set from memory.
my_set = {100, 200}
del my_set
# print(my_set)  # NameError: my_set is not defined
Set Mathematical Operations:
1. Union (| or union())

Combines two sets, removing duplicates.
Using | operator or .union() method.
A = {1, 2, 3}
B = {3, 4, 5}

print(A.union(B))  # -> or print(A | B)
{1, 2, 3, 4, 5}
2. Intersection (& or intersection())

Returns elements common to both sets.
Using & operator or .intersection() method.
A = {1, 2, 3}
B = {2, 3, 4}

print(A.intersection(B))  # -> or print(A & B)
{2, 3}
3. Difference (- or difference())

Returns elements in the first set but not in the second.
Using - operator or .difference() method.
A = {1, 2, 3, 4}
B = {3, 4, 5}

print(A.difference(B))  # -> or print(A - B)
{1, 2}
4. Symmetric Difference (^ or symmetric_difference())

Symmetric difference returns the all elements from both sets, excluding any elements common to both.
Using ^ operator or .symmetric_difference() method.
A = {1, 2, 3}
B = {3, 4, 5}

print(A.symmetric_difference(B))  # -> print(A ^ B)
{1, 2, 4, 5}
Set Relationships:
These operations help you compare sets, checking if one is a subset, superset, or if sets are completely disjoint.

Subset: A set A is a subset of a set B if all elements of A are also elements of B.
Superset: A set A is a superset of a set B if all elements of B are also elements of A.
Disjoint Sets: Two sets are disjoint if they have no elements in common.
1. Subset (issubset() or <=)

Returns True if all elements of Set A are in Set B

A = {1, 2}
B = {1, 2, 3, 4}

print(A.issubset(B))  # or print(A <= B)
True
2. Superset (issuperset() or >=)

Returns True if Set A contains all elements of Set B

A = {1, 2, 3, 4}
B = {2, 3}

print(A.issuperset(B))  # or print(A >= B)
True
3. Disjoint (isdisjoint())

Returns True if two sets have no elements in common

A = {1, 2, 3}
B = {4, 5, 6}

print(A.isdisjoint(B))
True
Subset → "I am part of the bigger group"

Superset → "I contain everything in the other group"

Disjoint → "We don’t share anything"

Looping Through a Set:
Since sets are unordered collections, you can loop through them using a simple for loop, but order is not guaranteed.

Basic for Loop
This prints all elements, in any order (not like list indexing)

fruit_set = {"apple", "banana", "cherry"}

for fruit in fruit_set:
    print(fruit)
cherry
banana
apple
Loop with Condition
my_set = {10, 20, 30, 40, 50}

for num in my_set:
    if num > 25:
        print(f"{num} is greater than 25")
50 is greater than 25
40 is greater than 25
30 is greater than 25
Frozenset
A frozenset is an immutable version of a set, meaning that once it is created, it cannot be modified (i.e., no adding or removing elements).
# creating frozenset
frozen_set = frozenset([1, 2, 3, 4, 5])
print(type(frozen_set))
print(frozen_set)
<class 'frozenset'>
frozenset({1, 2, 3, 4, 5})
6. Boolean Type
Represents one of two values: True or False.
Used for logical operations and conditions.
print(True)
print(False)
print(type(True))
True
False
<class 'bool'>
Boolean from Expressions:
print(5 > 3)      # True
print(10 == 20)   # False
print(3 < 7)      # True
print(5 != 5)     # False
True
False
True
False
bool() Function Conversio
Booleans in if Conditions:
x = 10
if x:
    print("x is truthy")  # Executes since 10 -> True
x is truthy
7. None Type
NoneType
Represents the absence of a value or a null value.
x = None
print(type(x))  # <class 'NoneType'>
<class 'NoneType'>
None
To initialize a variable without value
user = None
