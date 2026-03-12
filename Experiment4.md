# Experiment 4

## Aim
To write a Python program to create lists and perform various list operations using functions.

## Algorithm
1.Start the program.
2.Create a list of teams.
3.Display the original list.
4.Add a new element using append().
5.Add multiple elements using extend().
6.Insert an element at a specific position using insert().
7.Remove an element using remove().
8.Use pop() to remove an element by index.
9.Find the index of an element using index().
10.Count occurrences using count().
11.Display the final list.
12.Stop the program.

## Code
teams = ["India", "USA", "Pakistan", "Brazil", "South Africa", "Australia", "England"]
print("Original list:", teams)
teams.append("Bangladesh")
teams.extend(["Afghanistan", "Iraq"])
teams.insert(1, "Sri Lanka")
teams.remove("Iraq")
removed_item = teams.pop(3)
index_position = teams.index("USA")
count_sf = teams.count("South Africa")
print("Final list:", teams)
print("Removed item:", removed_item)
print("Index of USA:", index_position)
print("Count of South Africa:", count_sf)

## Output
Original list: ['India', 'USA', 'Pakistan', 'Brazil', 'South Africa', 'Australia', 'England']
Final list: ['India', 'Sri Lanka', 'USA', 'Brazil', 'South Africa', 'Australia', 'England', 'Bangladesh', 'Afghanistan']
Removed item: Pakistan
Index of USA: 2
Count of South Africa: 1

