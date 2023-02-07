# Modification-Floyd-Warshall
DSA II PROJECT (Individual Code)
Based on article "Modification of Floyd-Warshall’s Algorithm for Shortest Path Routing in Wireless Sensor Networks" by Pritam Khan, Gargi Konar, Niladri Chakraborty,[Modification_of_Floyd-Warshalls_algorithm_for_Shortest_Path_routing_in_wireless_sensor_networks.pdf](https://github.com/gfwltjd19/Modification-Floyd-Warshall/files/10673541/Modification_of_Floyd-Warshalls_algorithm_for_Shortest_Path_routing_in_wireless_sensor_networks.pdf)
 the purpose of the shortest path routing algorithm is to minimize the consumption amount of energy in a WSN. Floyd-Warshall’s Algorithm is used for computing shortest paths between different nodes in an ordinary graph instead of Djikstra as generally, Dijkstra’s Algorithm is used for routing through the shortest path in a WSN. But, the basic Floyd-Warshall’s algorithm is not exactly applicable for routing in wireless networks because of the absence of handshaking mode. The Floyd-Warshall’s Shortest Path Algorithm has been modified and a new algorithm has been proposed for routing in the wireless sensor networks. The proposed algorithm computes the shortest path available taking into consideration a directed graph and presence of acknowledgement path of every traversed path. This algorithm helps to obtain all the available shortest paths from every node to the other at a time.

Modified Floyd-Warshall’s Algorithm (Pseudocode): [Modified Floyd-Warshall’s Algorithm (Pseudocode).pdf](https://github.com/gfwltjd19/Modification-Floyd-Warshall/files/10673522/Modified.Floyd-Warshall.s.Algorithm.Pseudocode.pdf)


How to use the code (same for both code):
1.	Use Python compiler (Idle/ Google Colab/ Visual Studio Code) to run the code.
2.	Initialize number of vertices, n. 
3.	Initialize the value of weight for each edges (put 0 for self-loop, 999 for infinite distance or non-connectivity) using matrix.
4.  Run the code.

