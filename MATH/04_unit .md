Here’s a version of your note where the special LaTeX-style brackets and symbols have been replaced with simpler representations for better compatibility:

---

### **Graph Terminology**

1. **Graph (G)**:  
   A graph is a mathematical structure defined as a pair G = (V, E), where:  
   - **V**: Set of **vertices** (also called nodes).  
   - **E**: Set of **edges** (connections between vertices).

2. **Vertex (v)**:  
   An individual element in the set V.  
   - Example: v1, v2, etc.
  
    Isolated Vertex & Pendant Vertex: A vertex having 0 is called an isolated vertex and a vertex having degree 1 is called a pendant vertex.
 Finite and Infinite graph: A graph with a finite number of vertices as well as edges is called a finite graph otherwise it is an infinite graph.

3. **Edge (e)**:  
   A connection between two vertices.  
   - Represented as an ordered pair (in a directed graph) or an unordered pair (in an undirected graph).  
   - Example: (v1, v2) or {v1, v2}.

4. **Adjacency**:  
   Two vertices are **adjacent** if they are connected by an edge.  
   - Example: Vertices v1 and v2 are adjacent if there is an edge (v1, v2) or {v1, v2}.
   - 4.1 --- In graph theory, an adjacent edge refers to two edges in a graph that share a common vertex.

5. **Degree**:  
   The **degree** of a vertex is the number of edges incident to it.  
   - Degree of vertex v = Number of edges connected to v.  
   - For **directed graphs**:
     - **In-degree**: Number of edges directed into the vertex.  
     - **Out-degree**: Number of edges directed out of the vertex.

6. **Directed Graph (Digraph)**:  
   A graph where the edges have a direction (ordered pairs).  
   - Example: (v1, v2) indicates an edge from v1 to v2.

7. **Undirected Graph**:  
   A graph where the edges do not have a direction (unordered pairs).  
   - Example: {v1, v2} indicates an edge between v1 and v2, no direction.

8. **Path**:  
   A **path** is a sequence of edges that connects a sequence of vertices, where each vertex is visited only once.  
   - Example: v1 → v2 → v3 is a path.

9. **Cycle**:  
   A **cycle** is a path that starts and ends at the same vertex, without repeating other vertices.  
   - Example: v1 → v2 → v3 → v1.

10. **Connected Graph**:  
   A graph is **connected** if there is a path between every pair of vertices.

11. **Complete Graph**:  
   A **complete graph** is a graph where there is an edge between every pair of vertices.  
   - Example: In a complete graph with 3 vertices (K3), the edges are {(v1, v2), (v1, v3), (v2, v3)}.

12. **Null Graph**:  
   A **null graph** is a graph with no edges (E = empty set), but at least one vertex.  
   - Example: V = {v1, v2}, E = empty set.

13. **Singleton Graph**:  
   A graph with exactly one vertex. It may or may not have a self-loop.  
   - Example: V = {v1}, E = empty set or E = {(v1, v1)}.

14. **Subgraph**:  
   A **subgraph** is a graph formed by a subset of the vertices and edges of a larger graph.

15. **Isomorphism**:  
   Two graphs are **isomorphic** if there is a one-to-one correspondence between their vertices and edges, preserving adjacency.

16. **Bipartite Graph**:  
   A graph whose vertices can be divided into two disjoint sets, such that no two vertices within the same set are adjacent.

17. **Tree**:  
   A **tree** is a connected acyclic graph.  
   - It has no cycles and is connected.

18. **Spanning Tree**:  
   A **spanning tree** of a graph is a subgraph that includes all the vertices of the original graph and is a tree.

19. **Eulerian Path**:  
   A path in a graph that visits every edge exactly once.  
   - A graph has an Eulerian path if it has exactly 0 or 2 vertices of odd degree.

20. **Hamiltonian Path**:  
   A path in a graph that visits every vertex exactly once.

21. **Planar Graph**:  
   A **planar graph** can be drawn on a plane without any edges crossing.

22. **Graph Coloring**:  
   **Graph coloring** involves assigning colors to vertices or edges such that adjacent vertices (or edges) have different colors.

23. **Dijkstra’s Algorithm**:  
   A shortest-path algorithm that finds the shortest path from a source vertex to all other vertices in a weighted graph.

24. **Traveling Salesman Problem (TSP)**:  
   A problem of finding the shortest possible route that visits every vertex exactly once and returns to the starting point.

---

This version avoids LaTeX syntax and special characters, making it easier to copy-paste without issues. Let me know if you’d like further changes!
# ----------------------------------------------------------------

Here is the revised version with all special signs removed, formatted for direct copy and paste into a Markdown file:

---

### Graph Terminology

1. **Graph (G)**:  
   A graph is a pair G = (V, E), where:  
   - V = Set of vertices (nodes).  
   - E = Set of edges (connections between vertices).  

2. **Vertex (v)**:  
   An individual element in the set V.  
   - Example: v1, v2, etc.  

3. **Edge (e)**:  
   A connection between two vertices, represented as an ordered or unordered pair.  
   - Example: (v1, v2) or {v1, v2}.  

4. **Adjacency**:  
   Two vertices are adjacent if there is an edge connecting them.  
   - Example: If (v1, v2) is an edge, v1 and v2 are adjacent.  

5. **Degree**:  
   The degree of a vertex is the number of edges incident to it.  
   - In-degree: Number of edges directed into the vertex (for directed graphs).  
   - Out-degree: Number of edges directed out of the vertex (for directed graphs).  

6. **Self-loop**:  
   An edge that connects a vertex to itself.  
   - Example: (v1, v1).  

7. **Proper Edge**:  
   A proper edge is an edge that connects two different vertices.  
   - Example: (v1, v2), where v1 ≠ v2.  

8. **Multi-edge (Parallel Edge)**:  
   Multiple edges connecting the same pair of vertices.  
   - Example: Two edges (v1, v2) and (v1, v2) are parallel edges between v1 and v2.  

9. **Directed Graph (Digraph)**:  
   A graph where edges have a direction (ordered pairs).  
   - Example: (v1, v2) indicates a directed edge from v1 to v2.  

10. **Undirected Graph**:  
    A graph where edges do not have a direction (unordered pairs).  
    - Example: {v1, v2} indicates an edge between v1 and v2.  

11. **Weighted Graph**:  
    A graph where each edge has a weight (or cost) associated with it.  
    - Example: (v1, v2, 5) indicates an edge between v1 and v2 with weight 5.  

12. **Simple Graph**:  
    A graph without self-loops or multiple edges between any pair of vertices.  
    - Example: No multiple edges or loops are allowed.  

13. **Complete Graph**:  
    A graph where every pair of distinct vertices is connected by a unique edge.  
    - Example: A complete graph with 3 vertices, K3, has edges (v1, v2), (v1, v3), (v2, v3).  

14. **Null Graph**:  
    A graph with no edges, but it can have one or more vertices.  
    - Example: V = {v1, v2}, E = {}.  

15. **Disconnected Graph**:  
    A graph where not all vertices are connected by paths. There are disconnected components in the graph.  

16. **Connected Graph**:  
    A graph where there is a path between every pair of vertices.  

17. **Subgraph**:  
    A subgraph is a graph formed by selecting a subset of vertices and edges from a larger graph.  

18. **Isomorphic Graphs**:  
    Two graphs are isomorphic if there is a one-to-one correspondence between their vertices and edges, preserving the adjacency relationship.  

19. **Planar Graph**:  
    A graph that can be drawn in a plane without any edges crossing.  

20. **Regular Graph**:  
    A graph where every vertex has the same degree.  
    - Example: In a 3-regular graph, each vertex has degree 3.  

21. **Cycle**:  
    A path in which the starting and ending vertex is the same, without repeating any other vertices.  

22. **Path**:  
    A sequence of edges that connects a sequence of distinct vertices.  

23. **Cut**:  
    A partition of the vertices of a graph into two disjoint subsets.  

24. **Degree Sequence**:  
    The sequence of vertex degrees in a graph, arranged in non-increasing order.  

25. **Clique**:  
    A subset of vertices such that every pair of vertices in the subset is adjacent.  

26. **Independent Set**:  
    A set of vertices in a graph such that no two vertices in the set are adjacent.  

27. **Matching**:  
    A set of edges without common vertices. A maximum matching is a matching that includes the largest number of edges possible.  

28. **Graph Complement**:  
    The complement of a graph G = (V, E) is a graph G' with the same vertices but with edges that are not present in G.  

---  

This version is formatted for Markdown and ready for use. Let me know if any further changes are needed!

# Theorm 

the no of odd degree vertices in a graph is alwasy even 

Yes, it is true that **the number of vertices with an odd degree in any graph is always even**. This is a well-known result in graph theory, often referred to as the **Handshaking Lemma**.

### Why is this the case?
The **Handshaking Lemma** states that:

- The sum of the degrees of all vertices in a graph is **twice the number of edges**. 
  - This is because each edge contributes 1 to the degree of two vertices, so every edge is counted twice in the total degree sum.

### Formally:
If a graph has **n** vertices and **e** edges, the sum of the degrees of all the vertices is:
\[
\sum_{v \in V} \deg(v) = 2e
\]
This sum is **even**, because it is twice the number of edges.

Now, consider the degrees of the individual vertices:
- If a vertex has an **even degree**, it contributes an even number to the total sum.
- If a vertex has an **odd degree**, it contributes an odd number to the total sum.

For the total degree sum to be **even**, the number of vertices with an odd degree must be even, because the sum of an odd number of odd terms is odd, and the sum of an even number of odd terms is even.

Thus, **the number of vertices with an odd degree must always be even** to ensure the sum is even.

In every case, the number of vertices with an odd degree is always even.

Certainly! Here's the simplified version of your explanation in plain text format, ready for easy copy-pasting into Notepad:

---

**Simple Rule:**
- Even number of odd terms = Even sum
- Odd number of odd terms = Odd sum

**Example:**

1. **2 odd terms:**
   3 + 5 = 8 (even)

2. **3 odd terms:**
   3 + 5 + 7 = 15 (odd)

3. **4 odd terms:**
   1 + 3 + 5 + 7 = 16 (even)

4. **5 odd terms:**
   1 + 3 + 5 + 7 + 9 = 25 (odd)

---

