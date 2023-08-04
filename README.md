# mapping neighborhood states of cells to letters

can explore automata from the neighborhood state perspective not wether cell is alive or dead.  rule 25 and 89 produce the the longest string of non repeating states 7 of 8 states.   

I thought with more states say for a 6 bit you would have 32 states and map those states to letters you could have something like the library of Babble except it would not be random it would be deterministic


the neighborhood to rule size is like this:

The number of unique rule tables in a one-dimensional cellular automaton depends on the size of the neighborhood and the number of possible states for each cell. Let's generalize the problem:

If we have a one-dimensional cellular automaton with a neighborhood size of N (N is the number of neighboring cells), and each cell in the neighborhood can be in one of M states (M is the number of possible states for a cell), then the total number of unique rule tables can be calculated as:

Number of Unique Rule Tables = M^(M^N)

Let's break down the formula:

- M^N represents the total number of possible combinations of states for the N neighboring cells. Each neighboring cell can be in one of M states, so there are M possibilities for each cell, and N cells in the neighborhood lead to M^N combinations.

- M^(M^N) represents the number of possible mappings for the central cell. For each combination of states in the neighborhood (M^N possibilities), the central cell can be in one of M states. Thus, there are M^(M^N) possible ways to define the next state of the central cell for all combinations of its neighbors' states.

For the specific case of a 4-cell neighborhood (N = 4) and binary states (M = 2, on or off), the number of unique rule tables would be:

Number of Unique Rule Tables = 2^(2^4) = 2^16 = 65,536

So, in a one-dimensional cellular automaton with a 4-cell neighborhood and binary states, there would be 65,536 unique rule tables, each corresponding to a different configuration of how the central cell evolves based on the states of its four neighboring cells.

I am including the p5.min rather than cdn as will be coding this at times off line




https://greggelong.github.io/wolframLetter

 
on a torus 

note the changes with even and odd cell lengths per generation

as the Automaton is displayed on a torus overlaps in size produce different results even for regular patterns like rule 90

the overlaps are affected by size of the canvas and screen and wether or not the number of cells is even or odd

my favorite overlap for rule 90 

it produces something like a generative landscape 