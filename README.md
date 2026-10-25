# Task6-List-and-Dictionary-Comprehensions-in-Python
Overview
This project demonstrates how to create lists and dictionaries efficiently using Python comprehensions. It includes examples of transformation and filtering, which are useful in data preprocessing.
Objectives
Practice list comprehensions.
Practice dictionary comprehensions.
Filter and transform existing data.
Compare concise comprehensions with traditional loops.
Tools Used
Python
Jupyter Notebook
List Comprehension Examples
# 1. Squares of numbers
numbers = [1, 2, 3, 4, 5]
squares = [n ** 2 for n in numbers]
print(squares)

# 2. Even numbers (filtering)
evens = [n for n in numbers if n % 2 == 0]
print(evens)

# 3. Convert words to uppercase
words = ["python", "data", "science"]
upper_words = [word.upper() for word in words]
print(upper_words)

# 4. Length of each word
lengths = [len(word) for word in words]
print(lengths)

# 5. Pass marks only (filtering)
marks = [35, 78, 22, 90, 49]
passed = [mark for mark in marks if mark >= 35]
print(passed)
Dictionary Comprehension Examples
# 1. Number and its square
squares_dict = {n: n ** 2 for n in range(1, 6)}
print(squares_dict)

# 2. Student marks with pass/fail status
marks = {"Anu": 78, "Ravi": 28, "Sita": 90}
status = {name: ("Pass" if mark >= 35 else "Fail")
          for name, mark in marks.items()}
print(status)

# 3. Filter students who passed
passed_students = {name: mark for name, mark in marks.items()
                   if mark >= 35}
print(passed_students)
Basic Syntax
List: [expression for item in iterable if condition]
Dictionary: {key_expression: value_expression for item in iterable if condition}
The if condition is optional and can be used to filter items.
Conclusion
Comprehensions make Python code shorter and easier to read when creating collections, filtering values, and transforming data.
