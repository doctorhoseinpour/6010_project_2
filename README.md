# 6010 Project 2: Unsupervised Exploratory Graph Analysis of Communication and Recommendation Data

This repository contains the implementation, datasets, and Neo4j models used in an exploratory analysis of two large-scale graphs from distinct domains.  
Both datasets are **publicly available through the Stanford Network Analysis Project (SNAP)**:

- **[Email-Eu-core dataset](https://snap.stanford.edu/data/email-Eu-core.html)**: represents internal communication within a European research institution.  
- **[Amazon0302 dataset](https://snap.stanford.edu/data/amazon0302.html)**: represents product co-purchasing relationships on Amazon.  

The goal of this study is to analyze and compare the structural and behavioral properties of human communication networks and machine-driven recommendation systems using **Neo4j Desktop (v2.0.4)**.  
We focus on five fundamental graph properties: **in/out-degree distributions**, **reciprocity**, **node centrality measures**, and the combination of **number of triangles** and **clustering coefficient**.

---


### Folder Descriptions
- **Amazon_dataset/**  
  Contains the processed CSV files, Cypher queries, and the Neo4j import model for the Amazon co-purchasing network.

- **Email_dataset/**  
  Contains the processed CSV files, Cypher queries, and Neo4j import model for the email communication network.

---

## ⚙️ Neo4j Setup Instructions

Follow the steps below to import and explore the datasets in **Neo4j Desktop (v2.0.4)**:

1. **Install Neo4j Desktop (version 2.0.4)**  
   Download from [https://neo4j.com/download/](https://neo4j.com/download/).

2. **Create Two Databases**  
   - One for the **Email-Eu-core** dataset  
   - One for the **Amazon0302** dataset  

3. **Open the Import Page**  
   In Neo4j Desktop, go to the **Import** tab.

4. **Load the Import Model**  
   - Click **"Import Model"** and select the `neo4j_importer_model.json` file from the corresponding dataset folder.

5. **Upload CSV Files**  
   - Upload all CSV files (e.g., `edges.csv`, `departments.csv` for the email dataset) into the import page.

6. **Run the Import**  
   - Execute the import using the configured model.  
   - This will automatically create nodes and relationships according to the schema defined in the JSON model.

7. **Run the Queries**  
   - Use the queries provided in `Cypher_Queries.csv` to compute degree distributions, reciprocity, clustering, and other graph statistics.

---

## 🌐 Dataset Sources

Both datasets used in this analysis are **publicly available** through the **Stanford Network Analysis Project (SNAP):**

- **Email-Eu-core dataset:**  
  [https://snap.stanford.edu/data/email-Eu-core.html](https://snap.stanford.edu/data/email-Eu-core.html)

- **Amazon0302 dataset:**  
  [https://snap.stanford.edu/data/amazon0302.html](https://snap.stanford.edu/data/amazon0302.html)

---
