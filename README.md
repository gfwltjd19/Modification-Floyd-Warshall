# Modification-Floyd-Warshall
DSA II PROJECT (Individual Code)
Based on article "Modification of Floyd-Warshall’s Algorithm for Shortest Path Routing in Wireless Sensor Networks"

[DSA II readme.docx](https://github.com/gfwltjd19/Modification-Floyd-Warshall/files/10673482/DSA.II.readme.docx)
The purpose of the shortest path routing algorithm is to minimize the consumption amount of energy in a WSN. Floyd-Warshall’s Algorithm is used for computing shortest paths between different nodes in an ordinary graph instead of Djikstra as generally, Dijkstra’s Algorithm is used for routing through the shortest path in a WSN. But, the basic Floyd-Warshall’s algorithm is not exactly applicable for routing in wireless networks because of the absence of handshaking mode. The Floyd-Warshall’s Shortest Path Algorithm has been modified and a new algorithm has been proposed for routing in the wireless sensor networks. The proposed algorithm computes the shortest path available taking into consideration a directed graph and presence of acknowledgement path of every traversed path. This algorithm helps to obtain all the available shortest paths from every node to the other at a time.

Modified Floyd-Warshall’s Algorithm (Pseudocode):

Enter the input graph, number of vertices n and edges as parameters in a function, 
say mod_algo(p[][], n)
Repeat loop for i, j=1,2,…..,n:[Initializes q].
If  p[i,j]=0, then set q[i,j]=Infinity[say, 999]
else set q[i,j]=p[i,j]
[End of loop]
 Repeat loop for i, j=1, 2,…..,n.
If
q[i,j]=999 or q[j,i]=999, then set
q[i,j]=q[j,i]=999 [Validating a path in condition of presence of its corresponding acknowledgement path]
If q[i,j] and q[j,i] are not equal, then set
q[i,j]=q[j,i]=999 [Validating a path if its length equals that of reply path]
[End of loop]
Repeat Steps 5 and 6 for k=1, 2,………, n [Updates q]
Repeat Step 6 for i=1, 2, ….., n.
Repeat nested loop for j=1,2,…….,n.
Set q[i,j]=min(q[i,j], q[i,k]+q[k,j]).
[End of loop]
[End of Step 5 loop]
       [End of Step 4 loop]
Repeat loop for i=1, 2,…..,n.
Set q[i,i]=0 [Self-loops are absent]
[End of loop]
Print the final matrix q of shortest paths among all node-pairs.
Exit. 

How to use the code (same for both code):
1.	Use Python compiler (Idle/ Google Colab/ Visual Studio Code) to run the code.
2.	Initialize number of vertices, n. 
3.	Initialize the value of weight for each edges (put 0 for self-loop, 999 for infinite distance or non-connectivity) using matrix.
4.  Run the code.

