## Classes and Objects


1. What are Objects?

Objects are an encapsulation of variables and functions into a single entity. objects get thier variables and functions from classes, which are essentially a template to create your objects.

in my own words, Objects model certain person, place, or thing in programming, Classes are the factory that makes that definition of a person, place or thing!


Example of an object in Python:
"
cat = {"name":"Kayla", "breed":"Tortise Shell"}
"

example of a class in Python:
"
class MyClass:
    variable = "blah"

    def function(self):
        print("This is a message inside the class.")


"

myobjectx = MyClass()

To access the vairables or methods inside of the class you instantiated, just use dot notation!

myobjectx.variable

You can instantiate as many variables as you want, but to note, if you change the variable name inside the class it will only affect the last one you instantiated!



