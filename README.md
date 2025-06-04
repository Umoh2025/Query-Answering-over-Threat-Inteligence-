Efficient Query Answering over Threat Intelligence Knowledge Graphs

This repository presents a lightweight and effective framework for querying Threat Intelligence Knowledge Graphs (TIKGs) using Neo4j and manually crafted Cypher queries. The system is designed for cybersecurity analysts and researchers who seek structured, precise insights from complex cyber threat data. Focused on actors such as **SilverTerrier**, the framework supports analysis of Nigerian cyber threats by enabling semantic modeling of entities like threat actors, tools, techniques, and targeted organizations.
It supports data ingestion, graph construction, and query execution through a modular architecture, with visualization capabilities using Neo4j Browser.


Example Scenarios and Use Cases

This system allows users to turn natural-language questions into structured graph cypher queries. For instance, querying:  
“What tools has SilverTerrier used in BEC attacks?”  
is translated into Cypher and returns accurate tool names like *PhishX* and *Excel Macros*.  
Another query—“Which Nigerian organizations has SilverTerrier targeted between 2020 and 2024?”—returns key targets such as *FBN*, *GTB*, and *NIMC*.

These examples demonstrate how the system enables real-time investigation, campaign correlation, and actor profiling with interpretable outputs, either in tabular form or as interactive graph visualizations.


Application and Impact

The framework supports a wide range of applications, including **Threat Actor Profiling**, **Incident Investigation**, **Vulnerability Assessment**, and **Attack Forecasting**. Analysts can explore threat behaviors, trace malware campaigns, and predict future targets using graph-based reasoning. It also aids in **Security Awareness Training** and **Threat Reporting** by generating data-driven insights from structured CTI data. The system improves situational awareness, streamlines analyst workload, and enhances proactive cyber defense.


🔍 It is developed as part of academic research at Sharda University.  
📄 For more, see the full paper: *Efficient Query Answering over Threat Intelligence Knowledge Graphs (2025)*.
