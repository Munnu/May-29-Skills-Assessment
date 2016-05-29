#Skills-CS-Data-Struct
##Runtime
1. When calculating the Big O notation for a particular algorithm, it’s necessary to consider the length of time it takes for the algorithm to run as the algorithm’s workload approaches the size of infinity. What is the workload of a function that takes in a list of integers and returns a new list of the even integers? **O(n)**
2. Order the following runtimes in ascending order by efficiency as n approaches infinity:
	1. O(1) – Constant
	2. O(log(n)) – Log
	3. O(n) – Linear
	4. O(n*log(n)) – Log
	5. O(n^2) – Quadratic
	6. O(2^n) – Exponential

##Stacks and Queues
1. In the following cases, would a stack or queue be an appropriate data structure?
	1. The process of loading and unloading pallets onto a flatbed truck **Stack**
	2. Putting bottle caps on bottles of beer as they roll down an assembly line **Queue**
	3. Calculating the solution to this mathematical expression: 2 + (7 * 4) - (3 / 2) **Stack**
2. Describe 2 more examples of when a queue would be an appropriate data structure. 
	1. **typing words into a word processor document.**
	2. **A lunch line order**
3. Describe 2 more examples of when a stack would be an appropriate data structure.
	1. **Picking a card from the end of a deck**
	2. **Callstack**

##Linked Lists
1. Given the below linked list, which are the nodes? What is the data for each node? Where is the head? Where is the tail? (Please be as specific as possible — exactly which parts of the diagram correspond to each part? Arrows? Boxes? Text?)
	**Apple, Berry, Cherry, and their next pointers (and the none pointer for the tail) are nodes. Apple is the head of the linkedlist. Cherry is the tail. The next attributes are the pointers (the arrows in the diagram) to the linkedlist. Text is the data. The nodes are the boxes as diagrammed in the image.**
2. What’s the difference between a doubly and singly linked list?
**A doubly linked list contains in each node a pointer to the previous and the next.**
3. Why is it faster to append to a linked list if we keep track of the tail as an attribute?
**Because we have a reference to the tail at all times, and also we know that the tail does not have a pointer which means appending is faster.**

##Trees
1. Given the above tree, in what order would a Breadth First Search (BFS) algorithm visit each node until finding burrito (starting at food)?

	Food

	~~italian~~ indian mexican

	~~indian~~ mexican lasagna pizza

	~~mexican~~ lasagna pizza tikkamasala saag

	~~lasagna~~ pizza tikkamasala saag burrito tacos enchiladas

	~~pizza~~ tikkamasala saag burrito tacos enchiladas
	~~tikkamsala~~ saag burrito tacos enchiladas thin-crust chicago NY sicilian

	~~saag~~ burrito tacos enchiladas thin-crust chicago NY sicilian

	~~burrito~~ tacos enchiladas thin-crust chicago NY sicilian

2. Given the above tree, in what order would a Depth First Search algorithm visit each node until finding Chicago-style (starting at food)?

	Food
	
	italian indian ~~mexican~~
	
	italian indian burrito tacos ~~enchiladas~~
	
	italian indian burrito ~~tacos enchiladas~~
	
	italian indian ~~burrito tacos enchiladas~~
	
	italian tikka ~~saag~~
	
	italian ~~tikka saag~~
	
	lasagna ~~pizza~~

	lasagna thin-crust chiciago NY ~~sicilian~~

	lasagna thin-crust chiciago ~~NY sicilian~~
	
	lasagna thin-crust ~~chiciago NY sicilian~~

3. How is a binary search tree different from other trees?
**Binary search trees weigh in terms of order. The tree is arranged in terms of order. The left side holds items that are less than the right hand side.**