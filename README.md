📌 Overview

This project solves an optimization problem where the goal is to maximize profit under a fixed time constraint.
A land owner can construct different types of properties, each requiring a specific build time and generating income once completed.
Only one property can be built at a time, and earnings depend on the remaining operational time.

The solution uses Dynamic Programming to determine the optimal construction strategy.

🧩 Problem Statement

Mr. X owns unlimited land and can build one of the following properties:

Theatre (T)

Pub (P)

Commercial Park (C)

Each property:

Takes a fixed number of time units to construct

Starts generating income only after construction

Earns money for every remaining unit of time

Cannot be built in parallel with another property

Given a total time limit n, determine the maximum earnings and the optimal number of properties to build.

🏗 Property Details
Property	Build Time	Earnings per Unit Time
Theatre (T)	5	$1500
Pub (P)	4	$1000
Commercial Park (C)	10	$2000
🎯 Objective

Maximize total profit within n time units

Decide the optimal mix of properties

Output the count of Theatre, Pub, and Commercial Park

💡 Solution Approach
Dynamic Programming

Define dp[t] as the maximum profit achievable using t time units

At each time step, try building:

Theatre

Pub

Commercial Park

Choose the option that yields the highest profit based on remaining time

Backtrack to determine the number of each property built

This approach guarantees the optimal solution.

🧠 Algorithm Steps

Initialize a DP array to store maximum profit for each time unit

Iterate from 1 to n and compute the best profit

Store decisions to allow backtracking

Backtrack to count properties

Return total profit and property counts

⏱ Complexity Analysis

Time Complexity: O(n)

Space Complexity: O(n)

▶ Sample Input
Input Time Units: 7, 8, 13

✅ Sample Output
Input Time Unit: 7
Earnings: $3000
T: 1 P: 0 C: 0

Input Time Unit: 8
Earnings: $4500
T: 1 P: 0 C: 0

Input Time Unit: 13
Earnings: $16500
T: 2 P: 0 C: 0

🛠 Technologies Used

Python 3

Dynamic Programming

🌍 Real-World Applications

This problem reflects real-world resource and time optimization scenarios, such as:

Real Estate Development – deciding construction order for maximum rental income

Manufacturing Systems – scheduling machine installations

Cloud Infrastructure Deployment – prioritizing services that generate revenue sooner

Project Management – sequencing tasks for optimal returns

Operations Planning – maximizing output under time constraints# -Max-Profit-Optimization-Problem
📈 Max Profit Optimization Problem
