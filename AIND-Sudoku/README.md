# Artificial Intelligence Nanodegree
## Introductory Project: Diagonal Sudoku Solver

# Question 1 (Naked Twins)
Q: How do we use constraint propagation to solve the naked twins problem?  
A: By removing the values of the naked twins from the other boxes, we are shrinking the domain of the problem.  This is what constraint propagation is used for.  We took the sudoku problem, which had a rather large possible set of answers, and by removing some of the values we shrank that set bit by bit.  Because sudokus have such basic rules, you can use constraint proagation to remove values based on a set of rules.  We did this to remove all values from boxes that matched the values of the twins, because we know based on the rules that they would not be in those boxes. 

# Question 2 (Diagonal Sudoku)
Q: How do we use constraint propagation to solve the diagonal sudoku problem?  
A: Just like in all of the other units, if we include the diagonals, they have rules that limit the digits that can appear in them.  I just added the diagonals to the list of other diagonals, and the existing code worked perfectly with the diagonals, by now limiting the domain of possible answers for the sudoku.

### Install

This project requires **Python 3**.

We recommend students install [Anaconda](https://www.continuum.io/downloads), a pre-packaged Python distribution that contains all of the necessary libraries and software for this project. 
Please try using the environment we provided in the Anaconda lesson of the Nanodegree.

##### Optional: Pygame

Optionally, you can also install pygame if you want to see your visualization. If you've followed our instructions for setting up our conda environment, you should be all set.

If not, please see how to download pygame [here](http://www.pygame.org/download.shtml).

### Code

* `solutions.py` - You'll fill this in as part of your solution.
* `solution_test.py` - Do not modify this. You can test your solution by running `python solution_test.py`.
* `PySudoku.py` - Do not modify this. This is code for visualizing your solution.
* `visualize.py` - Do not modify this. This is code for visualizing your solution.

### Visualizing

To visualize your solution, please only assign values to the values_dict using the ```assign_values``` function provided in solution.py

### Data

The data consists of a text file of diagonal sudokus for you to solve.
