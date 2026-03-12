# Experiment 3

## Aim
To write a Python program to demonstrate various string operations.

## Algorithm
1.Start the program.
2.Input a string from the user.
3.Display the length of the string.
4.Convert the string to uppercase and lowercase.
5.Reverse the string.
6.Check if a substring exists in the string.
7.Display the results.
8.Stop the program.

## Code
s = input("Enter a string: ")
print("Original string:", s)
print("Length of string:", len(s))
print("Uppercase:", s.upper())
print("Lowercase:", s.lower())
print("Reversed string:", s[::-1])
sub = input("Enter substring to search: ")
if sub in s:
    print("Substring found")
else:
    print("Substring not found")

 ## Output
Enter a string: cat
Original string: cat       
Length of string: 3        
Uppercase: CAT
Lowercase: cat
Reversed string: tac       
Enter substring to search: i
Substring not found
