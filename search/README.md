# Documentation for Project1-part1-pacman
## 665 with Professor Ilmi Yoon
#### Student: Jonathan Dombrowski : 916921673

### Contents 
1. Overview 
2. File Structure 
3. How to Compile
4. Implementation discussion 
    1. DFS
    2. BFS
    3. UCS 
    4. A-star
5. Conclusion

### Overview 
The task assigned was to take the given code and extend the search methods to include DFS, 
BFS, UCS and A-star search methods. The rest of the game code was already supplied. Along 
with a suggested implementation of the node class and a suggested way of structuring the 
implementation such that we have general search problem that we simply change the object 
type and details of the fringe being passed. The implementation of the fringe ultimately 
decides the behavior of the search method. 

### File Structure
The two files that we were working in and using methods from were:

`search.py` ~ Where the different search methods were defined and the implementation of the 
`generalSearchProblem()`.  

`util.py` ~ Where the "data structures" that we are used to working with; ie: stack, queue, 
priority queue, are defined. The structures essentially build upon the predefined `list()` 
structure. It implements the `pop()` and `push()` methods that we are familiar with in order
to use with the Node implementation.

### How to Compile 

The compilation commands necessary are located in `search/commands.txt`

However, to run the autograder from CLI : `python search.autograder.py`

### Implementation
   
1. DFS
    
    Implemented a stack to traverse the deepest node first

2. BFS
	
	Implemented a queue traverse all children before going deeper in the tree 
	
3. UCS
	
	Implemented a priority queue to track and minimize the total path cost. The function utilized is simply the cost of the current_nodes' path. 
	 
4. A-star 

	Implemented a priority queue to track and minimize the total path cost. The function utilized is simply the cost of the current_nodes' path with an added heuristic that tracks the distance to the goal. So each step of the traversal will minimize the distance to the goal 
	
	
### Conclusion 

The general search problem was the most difficult portion because it involved debugging through the node structure and dealing with the fringe itself. Once that portion was completed, the rest of the search methods were straightforward. In the following questions, I am looking forward to working with other problem types and working with different heuristics. 