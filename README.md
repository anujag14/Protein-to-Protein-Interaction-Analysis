# Protein-to-Protein-Interaction-Analysis
This study presents a graph-based ML approach to predict cancer-related proteins using PPI networks. Key topological features feed classifiers (RF, SVM, XGBoost), with XGBoost achieving ~89% accuracy. SHAP highlights feature importance, and network analysis reveals disease modules, advancing cancer biomarker discovery.

Cancer is a multifaceted condition resulting from alterations in numerous genes, proteins, and pathways. In the current study, a new graph-based machine learning method for the prediction of cancer-related proteins based on protein-protein interaction (PPI) networks is explored. An integrated PPI network is constructed from meticulously curated databases, and its proteins are annotated on cancer relevance using biological databases. Key graph-theoretic features - degree, betweenness centrality, clustering coefficient, and community membership derived from its nodes serve as input to the classification models. Random Forest, Support Vector Machine, and XGBoost classifiers are trained and validated on these features to classify proteins based on their cancer-related status. The XGBoost algorithm performs the best and demonstrates a lot of predictive ability (accuracy approximately 89%, F1-score approximately 0.83) separating cancer-associated proteins, therefore clearly establishing that network topological features retain significant information pertinent to cancer relevance. In the spirit of interpretability, SHAP (SHapley Additive exPlanations) is applied to assess feature importance to ensure the strength of association of proteins of high network centrality with cancer. Network visualization tools are also employed to discover clusters, or "disease modules," of highly connected cancer proteins, revealing significant biological insights. The findings present evidence of the potential utility of graph-motivated features for cancer protein classification and solidify the potential of network medicine strategies. This dissertation outlines the method, places the work in contemporary literature, and points out contributions to the field of computational oncology, including an interpretable model of classification and results applicable for further advancements in biomarker discovery. Future work is outlined around multi-omics integration and active learning to refine the proposed model further and test its performance. Lastly, this research bridges the disciplines of bioinformatics and machine learning to advance our understanding of cancer biology from a network perspective.

Pairwise protein interactions that have been experimentally confirmed are included in the PPI dataset, along with UniProt IDs, synonyms, taxonomy IDs, interaction scores, experimental procedures, source databases, and PubMed references. To investigate connectivity and interaction strength, it serves as the foundation for building the protein interaction network. By providing functional details like protein and gene names, organism, sequence length, pathways, binding sites, and Gene Ontology terms, the UniProt protein annotation dataset allows the PPI network to be enriched for biological context analysis and functional classification.

Two datasets were used in this project:
* PPI.xlsx
* protein.xlsx

Technologies used:
* Python
* Graph Theory
* Network Topology
* NLP
* LSTM

https://snap.stanford.edu/biodata/datasets/10000/10000-PP-Pathways.html (Link for PPI dataset)
