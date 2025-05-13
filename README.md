# python_concept
Control Flow , Loops , Lists, Tuples , Dictionary , The Set & Frozenset


📘 Definition: Control Flow in Python
Control flow in Python refers to the order in which individual statements, instructions, or function calls are executed or evaluated.

Python provides control flow tools to make decisions, repeat actions, and control which parts of code are run based on conditions.

✅ Common Control Flow Statements:
if, elif, else – for decision making

for loops – for iterating over sequences

while loops – for repeated execution while a condition is true

break, continue, pass – for controlling loop execution

try, except – for handling errors (exception control flow)

----------------------------------------------------------------------------------------------------------------------------------------------------

🔁 Definition: Loops in Python
Loops in Python are used to execute a block of code repeatedly as long as a condition is met or while iterating over a sequence (like a list or range).

Loops help automate repetitive tasks without writing the same code multiple times.

✅ Types of Loops in Python:
for loop – used to iterate over a sequence like a list, tuple, string, or range.

while loop – keeps running as long as a condition is True.

Nested loops – a loop inside another loop.

Control statements within loops:

break – exits the loop early.

continue – skips to the next iteration.

pass – does nothing, used as a placeholder.

🔍 Why Loops Are Useful:
Automatically repeat tasks

Simplify code

Make programs efficient and scalable

---------------------------------------------------------------------------------------------------------------------------------------


📋 Definition: List in Python
A list in Python is an ordered, mutable (changeable), and iterable collection that can store multiple items in a single variable. Items in a list can be of any data type—strings, numbers, even other lists.

Lists are defined using square brackets:

my_list = [1, 2, 3, "apple", True]


✅ Key Features of Lists:
Ordered – Items have a fixed position (index starting from 0).

Mutable – You can add, remove, or change items.

Allows duplicates – Lists can contain repeated values.

Dynamic – You can grow or shrink them during runtime.

-------------------------------------------------------------------------------------------------------------------------------------



📦 Definition: Tuple in Python
A tuple in Python is an ordered, immutable (unchangeable) collection of items. Tuples are similar to lists, but unlike lists, you cannot change, add, or remove items once a tuple is created.

Tuples are defined using round brackets:
my_tuple = ("apple", "banana", "cherry")

✅ Key Features of Tuples:
Ordered – Items have a fixed order (starting from index 0).

Immutable – You cannot modify the tuple after creation.

Can contain mixed data types – integers, strings, booleans, etc.

Faster than lists – Ideal for fixed data that doesn’t change.

🔧 Common Tuple Operations:

colors = ("red", "green", "blue")

# Accessing items
print(colors[0])  # Output: red

# Looping through a tuple
for color in colors:
    print(color)

# Tuple unpacking
(r, g, b) = colors
print(r, g, b)  # Output: red green blue

# Checking membership
if "green" in colors:
    print("Green is in the tuple")
❌ Not Allowed:

# This will cause an error because tuples are immutable
colors[0] = "yellow"

----------------------------------------------------------------------------------------------------------------------------

📘 Definition: Dictionary in Python:-
A dictionary in Python is an unordered, mutable collection used to store data in key-value pairs.

Dictionaries are defined using curly braces {} with each item represented as a key: value pair.


person = {
    "name": "Asma",
    "age": 24,
    "is_student": True
}

✅ Key Features of Dictionaries:
Key-value pairs – each key must be unique.

Mutable – you can add, update, or remove items.

Unordered (in older Python versions) – but now maintains insertion order (since Python 3.7+).

Fast lookup using keys.


🔧 Common Dictionary Operations:

# Access value by key
print(person["name"])  # Output: Asma

# Add or update a key
person["email"] = "asma@example.com"

# Remove a key
del person["age"]

# Loop through keys
for key in person:
    print(key, ":", person[key])

# Check if key exists
if "name" in person:
    print("Name is in the dictionary")
    
📌 When to Use a Dictionary:
Use dictionaries when you want to label or associate values with meaningful keys—like user profiles, configuration settings, or storing structured data.

--------------------------------------------------------------------------------------------------------------------------------------------------------

🔷 Definition: Set in Python
A set in Python is an unordered, mutable collection of unique elements. Sets are useful when you want to store multiple items without duplicates and perform mathematical set operations like union, intersection, and difference.

Sets are defined using curly braces {} or the set() constructor:

my_set = {1, 2, 3}

✅ Key Features of Sets:
Unordered – no indexing or order guaranteed.

No duplicates – each item must be unique.

Mutable – you can add or remove items.

Efficient – fast membership testing and set operations.

🔧 Common Set Operations:

# Creating a set
fruits = {"apple", "banana", "cherry", "apple"}  # "apple" appears only once

# Add an item
fruits.add("orange")

# Remove an item
fruits.remove("banana")

# Check if item exists
if "apple" in fruits:
    print("Apple is in the set")

# Loop through set
for fruit in fruits:
    print(fruit)

# Set union
set1 = {1, 2, 3}
set2 = {3, 4, 5}
print("Union:", set1 | set2)

# Set intersection
print("Intersection:", set1 & set2)

# Set difference
print("Difference:", set1 - set2)
🚫 Not Allowed:

Sets do not support indexing like lists or tuples.
# This will raise an error
# print(fruits[0])

------------------------------------------------------------------------------------------------------------------------------------------------

🧊 Definition: frozenset in Python
A frozenset is an immutable version of a set. Like a regular set, it contains unique, unordered elements, but once created, you cannot change it—you can’t add or remove items.

It’s useful when you need a set that must not be modified, such as when using it as a key in a dictionary or storing it in another set.

✅ How to Create a frozenset:

# Create a frozenset
frozen = frozenset([1, 2, 3, 2, 1])
print(frozen)  # Output: frozenset({1, 2, 3})
🧩 Properties:
Immutable – cannot change after creation

Hashable – can be used as a key in a dictionary

Supports set operations like union, intersection, difference (returns new sets)

🔧 Example with Operations:
python
Copy
Edit
a = frozenset([1, 2, 3])
b = frozenset([3, 4, 5])

# Union
print("Union:", a | b)  # frozenset({1, 2, 3, 4, 5})

# Intersection
print("Intersection:", a & b)  # frozenset({3})

# Difference
print("Difference:", a - b)  # frozenset({1, 2})
🚫 Not Allowed:

a = frozenset([1, 2, 3])
# a.add(4)        ❌ Error: AttributeError
# a.remove(1)     ❌ Error: AttributeError

-------------------------------------------------------------***********************************-----------------------------------------------------------------
