# Applied Graph Theory and Network Science with Python

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue)](https://www.python.org/)
[![NetworkX](https://img.shields.io/badge/NetworkX-3.0%2B-blue)](https://networkx.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange)](https://jupyter.org/)

A comprehensive guide to graph theory and network science using Python and NetworkX. This repository contains Jupyter notebooks that cover fundamental concepts, algorithms, and applications of graph theory and network science.

## 📚 Table of Contents

1. [Getting Started](#-getting-started)
   - [Prerequisites](#prerequisites)
   - [Installation](#installation)
   - [Project Structure](#project-structure)
2. [Notebooks](#-notebooks)
3. [Contributing](#-contributing)
4. [License](#-license)
5. [Acknowledgements](#-acknowledgements)

## 🚀 Getting Started

### Prerequisites

- Python 3.8 or higher
- pip (Python package installer)
- Jupyter Notebook/Lab (included in the requirements)

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/applied_graph_theory_and_network_science_with_python.git
   cd applied_graph_theory_and_network_science_with_python
   ```

2. Create and activate a virtual environment (recommended):
   ```bash
   # Windows
   python -m venv venv
   .\venv\Scripts\activate
   
   # macOS/Linux
   python3 -m venv venv
   source venv/bin/activate
   ```

3. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```

4. Launch Jupyter Notebook/Lab:
   ```bash
   jupyter notebook
   # or
   jupyter lab
   ```

### Project Structure

```
applied_graph_theory_and_network_science_with_python/
├── data/                    # Data files
│   ├── raw/                 # Raw data files
│   └── processed/           # Processed data files
├── notebooks/               # Jupyter notebooks organized by topic
│   ├── 01_introduction/     # Introduction to graphs and NetworkX
│   ├── 02_networkx_basics/  # Basic NetworkX operations
│   ├── 03_graph_representation/  # Graph representations
│   ├── 04_graph_visualization/  # Graph visualization techniques
│   └── 05_graph_algorithms/     # Graph algorithms
├── .gitignore               # Git ignore file
└── requirements.txt         # Python dependencies
```

## 📓 Notebooks

The notebooks are organized in a progressive learning path:

1. **Introduction to Graphs**
   - Basic graph concepts
   - Graph types and properties
   - Real-world examples

2. **NetworkX Basics**
   - Creating and manipulating graphs
   - Node and edge attributes
   - Graph operations

3. **Graph Representation**
   - Adjacency lists and matrices
   - Edge lists
   - File I/O with different formats

4. **Graph Visualization**
   - Basic visualization with Matplotlib
   - Advanced layouts
   - Interactive visualization with Plotly

5. **Graph Algorithms**
   - Traversal algorithms (BFS, DFS)
   - Shortest paths
   - Centrality measures
   - Community detection

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgements

- NetworkX Development Team
- Jupyter Project
- Python Community
Chapter 4: Graph Visualization
The Importance of Visualization
Basic Visualization with NetworkX and Matplotlib
nx.draw() and its variations (draw_networkx, draw_circular, etc.)
Layout Algorithms (Spring, Circular, Random, Spectral, Kamada-Kawai)
Customizing Visualizations:
Node size, color, and labels
Edge width, color, and style
Using attributes for visual mapping
Challenges in Graph Visualization (Large graphs, hairball effect)
Introduction to other visualization libraries (e.g., Plotly, Bokeh, Gephi - brief mention)
Hands-on Exercises: Visualizing different types of graphs, experimenting with layouts, customizing appearance based on attributes.

Part 2: Core Graph Algorithms
Goal: Explore fundamental algorithms for analyzing graph structure and solving common problems.
Chapter 5: Traversal Algorithms
Exploring the Graph: Why Traversal Matters
Breadth-First Search (BFS)
Algorithm and Pseudocode
Implementation with NetworkX
Applications: Finding shortest paths in unweighted graphs, finding connected components.
Depth-First Search (DFS)
Algorithm and Pseudocode
Implementation with NetworkX
Applications: Cycle detection, topological sorting (for DAGs).
Hands-on Exercises: Implementing BFS/DFS traversals, finding components, detecting cycles.
Chapter 6: Shortest Paths
Defining Shortest Paths (Weighted and Unweighted)
Algorithms for Unweighted Graphs (BFS recap)
Dijkstra's Algorithm
Algorithm and Pseudocode (Priority Queue)
Implementation with NetworkX (nx.shortest_path, nx.dijkstra_path)
Handling weighted graphs
Bellman-Ford Algorithm
Handling negative edge weights
Detecting negative cycles
Implementation with NetworkX
A* Search Algorithm (Brief Introduction, Heuristics)
All-Pairs Shortest Paths (Floyd-Warshall, Johnson's Algorithm - brief mention and NetworkX functions)
Hands-on Exercises: Calculating shortest paths using different algorithms, applying to routing problems.
Chapter 7: Minimum Spanning Trees (MST)
Problem Definition: Connecting nodes with minimum total edge weight
Properties of MSTs
Prim's Algorithm
Algorithm and Pseudocode
Implementation with NetworkX
Kruskal's Algorithm
Algorithm and Pseudocode (Disjoint Set Union)
Implementation with NetworkX
Applications: Network design (e.g., laying cables), clustering (brief mention)
Hands-on Exercises: Finding MSTs using Prim's and Kruskal's algorithms, comparing results.
Chapter 8: Network Flows
Introduction to Flow Networks (Source, Sink, Capacities)
The Maximum Flow Problem
Ford-Fulkerson Algorithm and Edmonds-Karp Improvement (using BFS)
Residual Graphs and Augmenting Paths
Implementation with NetworkX
Max-Flow Min-Cut Theorem
Understanding Cuts
Relationship between flow and cuts
Applications: Logistics, resource allocation, network reliability, bipartite matching.
Hands-on Exercises: Calculating max flow, finding min cuts, modeling simple allocation problems.

Part 3: Network Structure and Analysis
Goal: Delve into methods for characterizing network structure, identifying important nodes, and understanding community formation.
Chapter 9: Centrality Measures
Identifying Important Nodes: What is Centrality?
Degree Centrality (Undirected and Directed)
Closeness Centrality
Definition and Interpretation
Handling disconnected components
Betweenness Centrality
Definition and Interpretation (Brokerage role)
Computational considerations
Eigenvector Centrality and PageRank
Influence in a network
Google's PageRank algorithm (conceptual overview)
Implementation of Centrality Measures in NetworkX
Choosing the Right Centrality Measure
Hands-on Exercises: Calculating various centrality measures for different networks, interpreting the results in context.
Chapter 10: Community Detection
What are Communities in Networks? (Clusters, Modules)
Measuring Community Structure: Modularity
Divisive Methods: Girvan-Newman Algorithm
Using edge betweenness
Algorithm steps
Agglomerative Methods: Louvain Method
Greedy modularity optimization
Algorithm steps (conceptual)
Other Approaches (Label Propagation - brief mention)
Implementation of Community Detection Algorithms in NetworkX (or related libraries like python-louvain)
Evaluating Community Structures
Hands-on Exercises: Applying community detection algorithms, visualizing communities, evaluating modularity.
Chapter 11: Network Models
Why Model Networks? Understanding formation mechanisms and properties.
Random Graphs: Erdős–Rényi Model (G(n, p) and G(n, M))
Properties: Degree distribution (Poisson), phase transitions
Generating with NetworkX
Small-World Networks: Watts-Strogatz Model
Properties: High clustering coefficient, low average path length ('six degrees of separation')
Generating with NetworkX
Scale-Free Networks: Barabási–Albert Model (Preferential Attachment)
Properties: Power-law degree distribution, hubs
Generating with NetworkX
Comparing Models to Real-World Networks
Hands-on Exercises: Generating graphs using different models, analyzing their properties (degree distribution, clustering, path length), comparing them.
Chapter 12: Special Graph Classes
Trees and Forests
Properties and characterizations
Algorithms on trees (e.g., traversals revisited)
Bipartite Graphs
Definition and properties
Checking bipartiteness (using BFS)
Algorithms: Maximum matching
NetworkX support for bipartite graphs
Planar Graphs (Brief Introduction)
Definition (Kuratowski's Theorem - mention)
Euler's formula
Directed Acyclic Graphs (DAGs)
Properties
Topological sorting revisited
Hands-on Exercises: Identifying graph types, testing bipartiteness, finding matchings, performing topological sorts.

Part 4: Applications and Advanced Topics
Goal: Showcase the application of graph theory and network science in various domains and introduce more advanced concepts.
Chapter 13: Social Network Analysis (SNA)
Modeling Social Relationships as Graphs
Identifying Key Players (Centrality revisited)
Community Structure in Social Networks (Echo chambers, groups)
Information Diffusion and Influence Maximization (Simple models)
Homophily and Assortativity
Case Studies: Analyzing real or synthetic social network data (e.g., Zachary's Karate Club)
Hands-on Project: Analyzing a social network dataset (e.g., from SNAP).
Chapter 14: Biological Networks
Types: Protein-Protein Interaction (PPI), Gene Regulatory Networks, Metabolic Networks
Representing Biological Systems as Graphs
Analyzing Network Motifs
Identifying Important Genes/Proteins (Centrality, essentiality)
Module Detection in Biological Networks
Using NetworkX for Biological Network Analysis
Hands-on Project: Analyzing a PPI network.
Chapter 15: Information and Technological Networks
The World Wide Web as a Graph (Nodes, links, structure)
Citation Networks (Analyzing scientific literature)
The Internet (Router/AS level topology)
Properties and Analysis (Power laws, small-world phenomena)
Ranking Algorithms (PageRank revisited)
Hands-on Project: Building and analyzing a small web crawl graph or citation network.
Chapter 16: Introduction to Advanced Topics (Optional/Brief Coverage)
Dynamic Networks and Temporal Graphs (Networks changing over time)
Multiplex and Multilayer Networks (Nodes connected by different types of relationships)
Graph Embeddings and Machine Learning on Graphs (Brief overview of concepts like Node2Vec, Graph Neural Networks)
Network Resilience and Robustness

Appendices
Appendix A: Python Fundamentals Refresher (Data structures, control flow, functions, classes - relevant to NetworkX usage)
Appendix B: Mathematical Concepts Review (Set theory, basic probability, matrix operations - relevant to graph theory)
Appendix C: NetworkX Function Reference (Quick guide to commonly used functions grouped by category)
Appendix D: Datasets for Network Analysis (Links to popular repositories like SNAP, KONECT, UCI Network Data Repository)
Appendix E: Further Reading and Resources (Classic textbooks, influential papers, online courses, software tools)

Each Chapter Structure:
Clear explanation of concepts and theory.
Illustrative examples.
Step-by-step implementation using NetworkX in Python.
Code snippets and explanations.
Hands-on exercises and potentially mini-projects.
Chapter summary and key takeaways.
Further reading suggestions.

