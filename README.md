### The-2021-Puzzle
### A* search with a suitable heuristic function 

State Space:- Any posssible board
Goal State: The Goal state for this problem is continuous arrangement of numbers from 1 to 20 in the form [[1,2,3,4,5],[6,7,8,9,10],[11,12,13,14,15],[16,17,18,19,20]] in the fewest possible number of possible moves.
Edge weights: The edge weights for any move for this problem is constant as the cost function function increases by only one no matter which possible step we take.
Successor function:- The successor function gives the set of all possible states that can be obtained when the successor function is applied to the current state, by moving 
		the respective row or column pertaining to the given constraints:sliding the first and third rows to the left only and the second and fourth rows to the right only and first,third and fifth columns can only be slid up and by sliding second and fourth columns to the down.

keep the intial board in fringe
pop the min cost value in fringe
get the successors for the poped out state and calculate cost and appened them to fringe til we get goal state.
we are not visiting the already visited staes if there cost function is more than existing cost function of that state

heuristic :- sum of manhattan distance of each element in a row and dividing it by 5 as there are 5 elements in row. + sum of manhattan distance for each element in column and dividing it by 4 as there are 4 elements in column.

cost function: 1+h(x)
