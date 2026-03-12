# Experiment 6

## Aim
To write a Python program to demonstrate dictionary operations and functions.

## Algorithm
1.Start the program.
2.Create a dictionary containing student details like name, age, subjects, and marks.
3.Display the original dictionary.
4.Add a new subject to the subjects list using append().
5.Update marks inside the nested dictionary.
6.Add a new key-value pair (city).
7.Update the age using update().
8.Access a value using get().
9.Display dictionary keys using keys().
10.Display dictionary values using values().
11.Display dictionary items using items().
12.Stop the program.

## Code
student={
    "name":"Daeen",
    "age":19,
    "subjects":["math","python","computer","networking",],
    "marks":{
        "math":85,
        "python":90
        }
    }
print("original dictionary")
print(student)
student["subjects"].append("english")
print(student)
student["marks"]["Math"] = 95
print(student)
student["city"] = "bangalore"
print(student)
print(student.update({"age": 20}))
print(student)
print(student.get("name"))
print(student.keys())
print(student.values())
print(student.items())

## Output
original dictionary
{'name': 'Daeen', 'age': 19, 'subjects': ['math', 'python', 'computer', 'networking'], 'marks': {'math': 85, 'python': 90}}
{'name': 'Daeen', 'age': 19, 'subjects': ['math', 'python', 'computer', 'networking', 'english'], 'marks': {'math': 85, 'python': 90}}
{'name': 'Daeen', 'age': 19, 'subjects': ['math', 'python', 'computer', 'networking', 'english'], 'marks': {'math': 85, 'python': 90, 'Math': 95}} 
{'name': 'Daeen', 'age': 19, 'subjects': ['math', 'python', 'computer', 'networking', 'english'], 'marks': {'math': 85, 'python': 90, 'Math': 95}, 
'city': 'bangalore'}
None
{'name': 'Daeen', 'age': 20, 'subjects': ['math', 'python', 'computer', 'networking', 'english'], 'marks': {'math': 85, 'python': 90, 'Math': 95}, 
'city': 'bangalore'}
Daeen
dict_keys(['name', 'age', 'subjects', 'marks', 'city'])
dict_values(['Daeen', 20, ['math', 'python', 'computer', 'networking', 'english'], {'math': 85, 'python': 90, 'Math': 95}, 'bangalore'])
dict_items([('name', 'Daeen'), ('age', 20), ('subjects', ['math', 'python', 'computer', 'networking', 'english']), ('marks', {'math': 85, 'python': 90, 'Math': 95}), ('city', 'bangalore')])
