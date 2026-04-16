# Experiment 8

# Aim
Program to demonstrate regular expressions and related functions in python

# Algorithm
1. start
2. import re module
3. define a text string
4. use finditer() to iterate over matches
5. use match() to check pattern at beginning
6. use search() to check first occurrence of pattern
7. use findall() to find all matches
8. use split() to split the strings
9. use sub() to repalce characters
10. use compile() to create pattern object and find matches
11. take input date from user
12. use fullmatch() to validate data format
13. display results and stop

# Code
import re

text = "My email is syeddaeeen@gmail.com and phone is 9611554404"

# 1. match()
pattern_match = r"My"
match_result = re.match(pattern_match, text)
if match_result:
    print("1. match():", match_result.group())
else:
    print("No match")

# 2. search()
pattern_search = r"\d{10}"
search_result = re.search(pattern_search, text)
if search_result:
    print("2. search():", search_result.group())
else:
    print("Not found")

# 3. findall()
pattern_findall = r"\w+@\w+\.\w+"
findall_result = re.findall(pattern_findall, text)
print("3. findall():", findall_result)

# 4. finditer()
print("4. finditer():")
for match in re.finditer(pattern_findall, text):
    print(f"Found: {match.group()} at position {match.start()}")

# 5. sub()
pattern_sub = r"\d"
sub_result = re.sub(pattern_sub, "*", text)
print("5. sub():", sub_result)

# 6. split()
pattern_split = r"\s"
split_result = re.split(pattern_split, text)
print("6. split():", split_result)

# 7. compile()
pattern_compile = re.compile(r"\w+")
compiled_result = pattern_compile.findall(text)
print("7. compiled pattern:", compiled_result)

# 8. fullmatch()
print("-" * 20)
date = input("Enter date (DD/MM/YYYY): ")
pattern_date = r"^\d{2}/\d{2}/\d{4}$"

if re.fullmatch(pattern_date, date):
    print("Valid date format")
else:
    print("Invalid date format")

# Output
1. match(): My
2. search(): 9611554404
3. findall(): ['syeddaeeen@gmail.com']
4. finditer():
Found: syeddaeeen@gmail.com at position 12
5. sub(): My email is syeddaeeen@gmail.com and phone is **********
6. split(): ['My', 'email', 'is', 'syeddaeeen@gmail.com', 'and', 'phone', 'is', '9611554404']
7. compiled pattern: ['My', 'email', 'is', 'syeddaeeen', 'gmail', 'com', 'and', 'phone', 'is', '9611554404']
--------------------
Enter date (DD/MM/YYYY): 29/07/2006
