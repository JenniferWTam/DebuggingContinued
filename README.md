# DebuggingContinued
Debugging Continued - Moira's Game of Life Code
Moira has been working on some code related to Conway's Game of Life  , but has run into some bugs. Today's task is to fork Moira's Replit and help Moira debug her code.

Before getting started, here is some important information about the project that Moira is working on:

Conway's Game of Life is a classic cellular automata  simulation in computer science. In Conway's Game of Life, there is a stage or grid, and each point in the stage is a cell. Each generation, every cell on the stage lives or dies based on a few simple rules.

Any live cell with < 2 neighbors dies
Any live cell with 2-3 neighbors lives
Any live cell with > 3 neighbors dies
Any dead cell with 3 neighbors comes alive
A cell's neighbors are the 8 cells immediately around the cell.

Before going further, take a minute to play with this Game of Life simulator  . Add a few points to the grid and press start to watch the simulation.

In today's project, Moira is testing her code using the Blinker pattern. The Blinker is an oscillator that flips from 3 vertical cells to three horizontal cells each generation:

A group of three blocks that alternates between a vertical and horizontal arrangement.
Fig. The oscillating shape called a blinker source 

Take a minute to make a Blinker in the simulator linked above and run it to verify its behavior.

Moira's project is to compute one generation of the Game of Life. She has been given functions that print the stage and calculate the number of neighbors of a cell. These functions are:

print_stage(stage)
count_neighbors(stage, x_pos, y_pos)
She has also been given the code that sets up the initial state of the stage with the 3 vertical cells of a Blinker (init_stage(stage)). Her task is to write the function one_generation(stage). If her function works, this sequence of function calls:

init_stage(stage)
print("First Generation:")
print_stage(stage)
one_generation(stage)
print("Second Generation:")
print_stage(stage)
will result in this output:

Two generations of output that depict a text representation of a blinker, oscillating from a vertical arrangement to a horizontal arrangement.
Fig. A text representation of a blinker across two generations

Before starting work, please fork Moira's Replit. Follow the link: https://replit.com/@adacore/DebuggingContdProblemSet  and click the Fork button to create a copy that you can edit.
