# Experiment 1

## Aim
To write a Python program to demonstrate branching statements (if, elif, else) using cricket player statistics.

## Algorithm
1.Start the program.
2.Input player statistics such as runs, balls, wickets, catches, and overs.
3.Calculate strike rate using runs and balls.
4.Calculate economy rate using runs and overs.
6.Use branching statements to evaluate batting and bowling performance.
7.Display the results.
8.Stop the program.

## Code
runs = int(input("Enter runs scored: "))
balls = int(input("Enter balls faced: "))
wickets = int(input("Enter wickets taken: "))
catches = int(input("Enter catches taken: "))
overs = float(input("Enter overs bowled: "))
strike_rate = (runs / balls) * 100
economy = runs / overs
print("Strike Rate:", strike_rate)
print("Economy Rate:", economy)
if strike_rate > 120:
    print("Excellent batting performance")
elif strike_rate > 80:
    print("Good batting performance")
else:
    print("Needs improvement in batting")
if economy < 6:
    print("Excellent bowling performance")
elif economy < 8:
    print("Average bowling performance")
else:
    print("Bowling needs improvement")

## Output
Enter runs scored: 50
Enter balls faced: 40
Enter wickets taken: 1
Enter catches taken: 2
Enter overs bowled: 4
Strike Rate: 125.0
Economy Rate: 12.5
Excellent batting performance
Bowling needs improvement   
