# Experiment 7

# To write a program to demonstrate classes and objects

# Algorithm
1. Start
2. create a class Student
3. define methods to get student details
4. define methods to display student details
5. create an object of the class
6. call methods to input, display data
7. stop

# Code
class student:
    def __init__(self, name, age):
        self.name = name
        self.age = age
    def display(self):
        print("Name:", self.name)
        print("Age:", self.age)
s1 = student("Daeen", 19)
s2 = student("Yash", 20)
s1.display()
print("----")
s2.display()   

# Output
Name: Daeen
Age: 19

----
Name: Yash
Age: 20
