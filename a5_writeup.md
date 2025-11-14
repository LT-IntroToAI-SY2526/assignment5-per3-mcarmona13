# Assignment 5 Write up

Assignment 5 can be broken up into the following parts:
1. Import the Necessary Modules:
- `copy`: For creating deep copies of objects
- `Stack` and `Queue`: Custom implementations for DFS and BFS operations
2. Utility Functions: 
- `remove_if_exists`: Removes a specified element from a list if it exists, which is used to remove the possibilites from a cell
3. Board Class:
- Represents the Sudoku board
- Consists of functions that will find the most constrained cell, and update the board, which eliminates possible solutions
4. DFS & BFS Functions:
- `DFS`: Uses depth-first search to solve the Sudoku puzzle. It works by trying to fill the most constrained cell with potential values until a solution is found or backtracks if a mistake is made
- `BFS`: Uses breadth-first search to solve the Sudoku puzzle in a similar fashion to DFS but explores nodes level by level
5. Main Execution:
- Defines two different sets of initial moves for Sudoku puzzles
- Uses both DFS and BFS to solve each puzzle and prints the results


After completing the assignment, answer the following reflection questions:

## Reflection Questions

1. What are some things that you learned through this assignment? Think about the concepts of backtracking, constraint satisfaction, and search algorithms. Were there any particular challenges you faced while implementing the Board class methods or the DFS/BFS functions? How did you overcome them?

I learned how backtracking works by tryng different numbers & going back when I hit dead end. The hardest part was keeping track of the nested lists and remembering to copy the board before making changes, otherwise all of my boards would get mixed up. I also learned that choosing the cell with the fewest options first makes solving faster. 


2. How can you apply what you learned in this assignment to future programs or projects? Consider other types of problems that involve searching through possibilities, making decisions, and backtracking when those decisions don't work out. Can you think of real-world scenarios where DFS or BFS might be useful? What about other constraint satisfaction problems?

These ideas could help solve problems like creating class schedules without time conflicts or planning routes through a maze. DFS goes deep into one option before trying others, which is good for quickly finding any answer, while BFS checks all nearby options first, which finds the shortest path. I could use these things like solving other puzzles, planning trips, or organizing tasks with dependencies. 

3. Explain how the Stack and Queue classes work and why they are important for DFS and BFS algorithms. Describe the difference between LIFO (Last In First Out) and FIFO (First In First Out) data structures. How does using a Stack versus a Queue change the way the search algorithm explores possible solutions? Why is one data structure better suited for depth-first search and the other for breadth-first search?

A stack works like a pile of plates where you only add or take from the top(last thing in, is the 1st thin out), while a queue works like a line where you join the back & leave form the front(first thing in, is 1st thing out). DFS uses a stack so it explores older possibilities first & spreads out even;y. The data structure you pick completely changes which path get explored first.