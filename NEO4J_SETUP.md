
## 🧩 Neo4j Setup and Usage Guide

To replicate the graph-based threat intelligence analysis described in this project, follow these steps to download, install, and use **Neo4j**:

### 📥 Step 1: Download Neo4j

You can choose between two main options:

- **Neo4j Desktop (Recommended for development):**  
  Download from: [https://neo4j.com/download/](https://neo4j.com/download/)

- **Neo4j Aura (Cloud-based):**  
  Register and use: [https://neo4j.com/cloud/aura/](https://neo4j.com/cloud/aura/)

### 💻 Step 2: Install and Start Neo4j

1. **Install Neo4j Desktop** by following the setup wizard.
2. Open Neo4j Desktop and **create a new project**.
3. Inside the project, **create a new database**, give it a name (e.g., `TIKG`), set a password (e.g., `neo4j1234`), and start it.
4. You’ll get a **Bolt URI** like `bolt://localhost:7687` which will be used in the Python scripts.

### 🛠️ Step 3: Configure Your Environment

Update the Neo4j connection settings in your Python script:
```python
from py2neo import Graph
graph = Graph("bolt://localhost:7687", auth=("neo4j", "neo4j1234"))
```

Install Python dependencies:
```bash
pip install py2neo pandas networkx
```

### 🌐 Step 4: Use the Framework for Graph Generation

1. Load your data and generate the knowledge graph:
```bash
python src/graph_builder.py
```

2. Run Cypher queries using the pre-written scripts or via Neo4j Browser:
```bash
python src/query_runner.py --query queries/silver_terrier_targets.cypher
```

3. Visualize and explore the graph structure in **Neo4j Browser** by visiting:
[http://localhost:7474](http://localhost:7474)

---

For more advanced usage, refer to Neo4j documentation:  
📚 [Neo4j Developer Docs](https://neo4j.com/docs/)
