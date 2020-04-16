# Python Practice

## Variables

We use variables to store data in the computer's memory e.i.:

	students_count = 10

when we run this program Python interpreter will allocate some memory and store this number 10 in that memory space. then it will have this variable reference that memory location, in other words, this variable is just like a label for that memory location.

### Built-in primitive types in Python

	# Numbers
	students_count = 10
	rating = 4.99

	# Booleans
	is_published = True

	# Strings
	course_name = "Python training"

## Variable names

In the above example, you can notice that all variable names are descriptive and meaningful.

## Strings

We use double quotes for declaring a string variable. We also have triple quotes and we use them to format a long string e.g:

	course = "Python training" 

	message = """ 
	Hi John,

	This is a message send from the Globant team...

	blah blah blah
	"""

Triple quotes are useful when we writing the body of an email.

### Built-in functions

	course = "Python training"

	print(len(course))

	print(course[0])

	print(course[-1])

	print(course[-2])

	print(course[0:3])

	print(course[0:])

	print(course[:3])

	print(course[:])

	Terminal:
	15
	P
	g
	n
	Pyt
	Python training
	Pyt
	Python training

## Escape sequences

What if we wanna display the following message with double quote in the middle of the string:

	course = "Python "training"

Python interpreter will take the second double quote as the end of the string, so the rest of the string (**training"**) it's meaningless and invalid.

**Two way to resolve this problem**

Using single quotes
	course = 'Python "training'

Prefix with a backslash
	course = "Python \"training"

Backslash in Python string is a special character. We have jargon for that called *escape character* and is used to scape the character after.	

	print('Python "training')

	print("Python \"training")
	print("Python \'training")
	print("Python \\training")
	print("Python \ntraining")

	Terminal:
	Python "training
	Python "training
	Python 'training
	Python \training
	Python 
	training

## Format Strings

	first = "John"
	last = "Doe"
	full = f"{first} {last}"

	print(full)

	Terminal:
	John Doe

	first = "John"
	last = "Doe"
	full = f"{len(first)} {last} {2 + 6}"

	print(full)

	Terminal:
	4 Doe 8

## Strings Methods

Something that you need to take away is that in Python everything is an object and objects have functions we call methods that we can access using the dot notation.

	course = "python training"
	print(course.upper)

	Terminal:
	PYTHON TRAINING

**Important** the methods that we call return a new string, so the original string is not affected, let's see that in the example below:

	course = "python training"
	print(course.upper())
	print(course)

	Terminal:
	PYTHON TRAINING
	python training

There are few more string methods you can access them using the dot notation.
