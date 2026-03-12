# Experiment 5

## Aim
To write a Python program to demonstrate tuple operations and functions.

## Algorithm
1.Start the program.
2.Create a tuple with some numbers.
3.Display the original tuple.
4.Access the first and last elements using indexing.
5.Find the length of the tuple using len()
6.Find the maximum and minimum values using max() and min().
7.Find the sum of elements using sum().
8.Find the index of an element using index().
9.Perform tuple slicing.
10.Concatenate another tuple.
11.Display the final tuple.
12.Stop the program.

## Code
numbers = (10, 20, 30, 40, 20, 50)
print("Original Tuple:", numbers)
print("First element:", numbers[0])
print("Last element:", numbers[-1])
print("Length of tuple:", len(numbers))
print("Maximum value:", max(numbers))
print("Minimum value:", min(numbers))
print("Sum of elements:", sum(numbers))
print("Index of 30:", numbers.index(30))
print("Tuple slicing (1 to 4):", numbers[1:4])
tuple2 = (60, 70)
new_tuple = numbers + tuple2
print("After concatenation:", new_tuple)

## Output
First element: 10
Last element: 50
Length of tuple: 6
Maximum value: 50
Minimum value: 10
Sum of elements: 170
Index of 30: 2
Tuple slicing (1 to 4): (20, 30, 40)
After concatenation: (10, 20, 30, 40, 20, 50, 60, 70)

