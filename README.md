# Game of life Explanation

# Input From User:
1. Get the Grid Size through Console
2. Get Total Future Generation, through Console,  we want to perform this operation.


# Working Approach:
1. Once Seed of the System randomly generated, or we can also define initial state.
2. This will work as input for next Generation, and further on.
3. For every cell, it would've total 08 neighbors, and we've to find total live_neighbors.
4. Based on live_neighbors, we've defined operations. Accordingly, we can change state
5. If current cell is Alive, and live_neighbors less than 02, or greater than 03, then we've changed current cell with -1
    It'll work as flag and indicate once iteration is done for current generation, make it to dead cell for next generation.
    And we'll use it's absolute function while evaluating current generation for other neighbours cells.
    And once we've done with iteration for current generation, we'll change with correct value with 0.
    This Approach will help us not to use extra memory space(or 2-D array for storing temporary calculation).
6. If current cell is Alive, and live_neighbors are exactly 02 or 03, then there is no change in the Grid.
7. If current cell is Dead, and live_neighbors are exactly 03, then we've changed current cell with 2. 
    it will indicate that once iteration is done for current generation, we'll make it Alive cell, replace with correct value 1.


# Output For Each Generation
1. Output for each generation including Seeds of the System will be printing in the console only.
