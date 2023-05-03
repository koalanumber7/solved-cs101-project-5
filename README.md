Download Link: https://assignmentchef.com/product/solved-cs101-project-5
<br>
Suppose that you are searching for an airline flight.  You will be interested in the price of the flight, but you will probably also be interested in the amount of time that the flight(s) will take.  This program is based on that problem.  You will be given a directed graph where each edge has a cost and a duration.  Your job will be to find the shortest duration path in the graph that doesn’t go over a given maximum cost.

The graph will be given as follows: the number of vertices and edges will be on the first line, followed by one edge per line.  Each edge will list the two vertices, the cost and the duration, all of which will be positive integers.  Note that in this graph there may be multiple edges between any two vertices.

Your program should take four command line arguments:  the name of the file containing the graph, the start vertex, the destination vertex, and the maximum total cost.  The output of the program is the duration and cost of the path from start to destination, along with the path itself.  If no path exists with cost less than the limit, output the words “No path”.  No other output should appear.




Hint: for this program, you will want to modify the Bellman-Ford algorithm.  Instead of a single distance for each vertex of the graph, you will need to maintain an ordered list based on cost.




Example input graph:

5 7

0 1 30 100

<ul>

 <li>4 50 125</li>

 <li>2 250 50</li>

</ul>

1 2 50 150

4 2 40 100

2 3 60 90

4 3 150 125




Executing p6.exe graph.txt 0 3 200 Should output:

Cost 200  Duration 250

Path 0, 4, 3




Executing p6.exe graph.txt 0 3 145 Should output:

Cost 140 Duration  340

Path 0, 1, 2, 3




Executing p6.exe graph.txt 0 3 139 Should output:

No path


