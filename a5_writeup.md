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

1. How do the performance and efficiency of the Depth-First Search (DFS) and Breadth-First Search (BFS) algorithms compare when solving Sudoku puzzles? In what scenarios might one approach be preferable over the other?

The DFS algrotihm is more efficient than the BFS algroithm because it solves the puzzle using fewer iterations. The DFS had 87 iterations while the BFS had around 543 iterations. DFS is more efficient for situations where the stored data is deeper and more complex while the BFS would work better for data that stores lots of information but doesn't go in depth. DFS would work better for scenarios involving graphs or trees with different branches extending off of it. 


2. How did the choice of data structures (like the Stack for DFS and Queue for BFS) impact the implementation and functionality of the algorithms? Are there alternative data structures or design patterns that could have been used to achieve the same objectives?

Using data structures organizes the code. For the sudoku puzzle, it is better to use a stack for DFS because the puzzle has many extending branches and many possible solutions to go over. When you search for one solution more possibilities pop up. Using a queue is better for BFS because it allows you to look at all possible solutions. 




3. Considering the current implementation, how might the Sudoku solver be adapted or extended for larger puzzles or different types of grid-based logic games? How can the lessons learned from this assignment be applied to real-world problem-solving or optimization challenges?

This code could be implemented to solve any problem that has multiple possibilities. I learned the difference between BFS and DFS and how to implement them, which could be used to solve a rubiks cube or when playing chess, to decide which moves have the highest victory percentage. 