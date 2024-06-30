# Remove Max Number of Edges to Keep Graph Fully Traversable

LeetCode Q # 1579.

Alice and Bob have an undirected graph of n nodes and three types of edges:

- Type 1: Can be traversed by Alice only.</br>
- Type 2: Can be traversed by Bob only.</br>
- Type 3: Can be traversed by both Alice and Bob.</br>
Given an array edges where edges[i] = [typei, ui, vi] represents a bidirectional edge of type typei between nodes ui and vi, find the maximum number of edges you can remove so that after removing the edges, the graph can still be fully traversed by both Alice and Bob. The graph is fully traversed by Alice and Bob if starting from any node, they can reach all other nodes.</br>

Return the maximum number of edges you can remove, or return -1 if Alice and Bob cannot fully traverse the graph.

Example 1:

<div align = "center">

  ![image](https://github.com/xo-azeem/Remove-Max-Number-of-Edges-to-Keep-Graph-Fully-Traversable-LeetCode/assets/171427226/ddeb76b5-4a0f-44b2-9fd5-84a362c135b4)

</div>

> Input: n = 4, edges = [[3,1,2],[3,2,3],[1,1,3],[1,2,4],[1,1,2],[2,3,4]]</br>
> Output: 2</br>
> Explanation: If we remove the 2 edges [1,1,2] and [1,1,3]. The graph will still be fully traversable by Alice and Bob. Removing any additional edge will not make it so. So the maximum number of edges we can remove is 2.

Example 2:

<div align = "center">

  ![image](https://github.com/xo-azeem/Remove-Max-Number-of-Edges-to-Keep-Graph-Fully-Traversable-LeetCode/assets/171427226/2297e096-ec72-4ac3-a9ca-6df9a78af44c)

</div>

> Input: n = 4, edges = [[3,1,2],[3,2,3],[1,1,4],[2,1,4]]</br>
> Output: 0</br>
> Explanation: Notice that removing any edge will not make the graph fully traversable by Alice and Bob.

Example 3:

<div align = "center">

  ![image](https://github.com/xo-azeem/Remove-Max-Number-of-Edges-to-Keep-Graph-Fully-Traversable-LeetCode/assets/171427226/549ff6a3-792d-4cce-9b99-3313642964ff)

</div>

> Input: n = 4, edges = [[3,2,3],[1,1,2],[2,3,4]]</br>
> Output: -1</br>
> Explanation: In the current graph, Alice cannot reach node 4 from the other nodes. Likewise, Bob cannot reach 1. Therefore it's impossible to make the graph fully traversable.

My Solution Analysis:

<div align = "center">

  ![image](https://github.com/xo-azeem/Remove-Max-Number-of-Edges-to-Keep-Graph-Fully-Traversable-LeetCode/assets/171427226/22dd7a12-ca4e-4e8c-a3cd-7e7ba726b169)

</div>
