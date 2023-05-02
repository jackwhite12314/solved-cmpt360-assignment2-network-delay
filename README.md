Download Link: https://assignmentchef.com/product/solved-cmpt360-assignment2-network-delay
<br>
Assume that a large database is being transferred from a source <em>S </em>to a destination <em>D</em>. The transfer is being done through many routes in the form of small data packets. The destination puts the data packets on a stack in the order they arrive. Since different paths have different time requirement, a set of packets <em>p</em><sub>1</sub><em>,p</em><sub>2</sub><em>,p</em><sub>3</sub><em>,p</em><sub>4</sub><em>,p</em><sub>5 </sub>may be collected at <em>D </em>in the order <em>S </em>= (<em>p</em><sub>3</sub><em>,p</em><sub>1</sub><em>,p</em><sub>5</sub><em>,p</em><sub>4</sub><em>,p</em><sub>2</sub>).

A network performance metric <em>t </em>for this data transfer is computed by taking for every pair of packets <em>p<sub>i</sub>,p<sub>j </sub></em>∈ <em>S</em>, where <em>p<sub>i </sub></em>arrives before <em>p<sub>j</sub></em>, the maximum of (<em>i </em>− <em>j</em>). In the above example, <em>t </em>= 3, which is determined by <em>p</em><sub>5 </sub>and <em>p</em><sub>2</sub>

<strong>Input:</strong>

The input is in ‘network.txt’. Each line contains a list of <em>n </em>numbers (1 ≤ <em>n </em>≤ 1<em>,</em>000) representing the packet ordering at <em>D</em>. <strong>Sample input:</strong>

3,1,5,4,2

10,3,200

<strong>Output:</strong>

Each line of the output contains one number, which is the performance metric for the corresponding input.

<strong>Sample output:</strong>

3

7

<strong>Instructions:</strong>

Edit the given code Network.java to complete the assignment. Do not edit the part which is READ ONLY. Only submit Network.java in Moodle. To obtain a full mark for this question, you must try to achieve an <em>O</em>(<em>n</em>log<em>n</em>) time algorithm.

<h1>B. Mass Production of Quantum Computer</h1>

This is expensive, so before the production – we want to find the best possible design.

The specification says that the computer has <em>X </em>‘data bus’ — you can think this as <em>X </em>parallel and disjoint horizontal lines lying on the lines <em>y </em>= <em>k</em>, where 1 ≤ <em>k </em>≤ <em>X</em>.

The computer needs to connect each pair of buses. The connections can only be vertical. The cost of connecting a pair of buses is the number of other buses that it crosses. The task is to find the minimum total cost for arranging the buses.

Figure A is showing a configuration with cost 1, and this is the minimum possible when <em>X </em>= 5. Note that there can be exactly 10 possible connections for 5 buses and we can make 9 of these connections without crossing. The one shown in red is the one where there is no way we can avoid a crossing.

Figure B is showing a configuration with cost 3, where <em>X </em>= 6. I am not going to tell you whether this is the minimum possible – ask others in piazza.

Although in the above examples each connection crosses at most one bus, for larger values of <em>X</em>, a minimum cost solution may contain a connection with two or more buses.

<strong>Input:</strong>

The input is in ‘quantum.txt’. Each line contains a number <em>X</em>, representing the number of data buses.

<strong>Sample input:</strong>

1

4

5

<strong>Output:</strong>

Each line of the output contains one number, which is the cost for the corresponding input. <strong>Sample output:</strong>

0

0

1

<strong>Instructions:</strong>

Edit the given code Quantum.java to complete the assignment. Do not edit the part which is READ ONLY. Only submit Quantum.java in Moodle. To obtain a full mark for this question, you must try to achieve answers for larger values of <em>X</em>.

<strong>Reward:</strong>

If you can find a correct answer for <em>X </em>= 8, then you get a reward. You can submit for a reward anytime before November 30.

<h1>C.         Just to Sharpen the Brain</h1>

Let’s define a class of graphs called ‘Recursive Network’ consisting of <em>n </em>≥ 4 nodes. The base graph looks like the top left graph in the following figure. The subsequent graphs are produced by inserting new nodes in clockwise order.

Given a recursive network, we want to find a crossing free layout for the graph minimizing rectangular area of the layout. The term ‘crossing free’ means no two links cross in the layout.

The bottom figure shows an example crossing free layout that minimizes the area when <em>n </em>= 7. The rectangular area is (width × height) of the layout. In this example, the area is <sub>3</sub>×<sub>6 = 18 </sub>unit square, which is the best possible.

<strong>Instructions:</strong>

Write your answer and upload a single pdf in moodle. Your answer must consist the followings.

<ul>

 <li>A recurrence relation for solving the problem using dynamic programming.</li>

 <li>A pseudocode for solving the problem using your recurrence relation.</li>

 <li>A brief argument of why you think your algorithm will produce a correct answer.</li>

 <li>The description of the dynamic programming table (or data structure, if any) thatyou will be using.</li>

 <li>Time complexity analysis of your dynamic programming.</li>

</ul>

To get a full mark, your algorithm must have a time complexity, which is a polynomial in <em>n</em>.

<strong>Reward:</strong>

If you can find a correct answer with a running time around <em>O</em>(<em>n</em><sup>9</sup>), then you will get a bonus.

Here <em>n </em>is the number of nodes. You can submit for a reward anytime before November 30.