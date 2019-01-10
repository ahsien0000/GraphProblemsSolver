## Graph-based problems

In graph theory, there are multiple classic optimization problems, such as shortest path problem, minumum spanning tree problem, flow problem, etc. Here I implemented a python-version problem solver program , for user to import a graph with .csv file, choose corresponding algorithms, and obtain the problem result. 

### Python NetworkX Library

NetworkX provides basic functions for generating graphs including nodes and edges, and also provides functions API for developers to call.
For exampl:
```
    import networkx as nx
    ...
    G = nx.DiGraph()
    ...
    nx.dfs_edges(G, source=0, depth_limit=int(n))
```

### TkInter

Applied TkInter library in Python to visulize the problem solver.


### Graph format

The graph format we use here is comma-separated values file (.csv). In this repo you may find a sample graph.csv file, and you can extend/manupulate the file before you want to import the file into the program. Each row(tuple) in the file represents an edge in the graph. There are three columns, source, target, and weight, such that source and target indicate the direction of each edge, and weight is the cost on the edge.
For example:
```
    source,target,weight
    0,      1,      1
    0,      2,      2
    0,      3,      1
```

### Reference

1. https://networkx.github.io/documentation/stable/reference/algorithms/index.html


### Support or contacts
[contact support](chunghc3@uci.edu), and we’ll help you sort it out.
