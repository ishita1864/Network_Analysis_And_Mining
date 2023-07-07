# Network_Analysis_And_Mining
Lab Assignments for the Network Analysis and Mining Course


Evaluation 1:

Implementation (6 marks) : (a) Make a list of characters in the novel. You need to decide whom to include.

(b) Extract a social graph of the manually identified characters in the text ( as shown in the hands on session) . For doing this, you need to use a co-occurrence algorithm as discussed and shown in demo in class

(c) Calculate the four types of centrality of main protagonists i.e. degree, betweenness, closeness, PageRank . (Ref : Unit 1 – centrality analysis)

(d) Calculate the global clustering coefficient of your graph and local clustering coefficient of the main protagonist nodes. Detect communities ( Ref : Unit 2 – Measures of cohesion)

(e) Find the degree distribution, average shortest path, size of the largest component. Also create an equivalent generative model to compare against the social graph that you extracted (Ref : unit 3 - Generative models)

Analysis ( 4 marks) -

Theme of the analysis: What you know of the story and is it matching with what you got from your network analysis ? Have you got any insight to offer ?

Evaluation 2:

TITLE: Comparative Analysis of Traditional Methods and Graph Machine

Learning Methods for Link Prediction

GOAL To compare traditional, similarity-based methods with GraphML algorithms like GCN, GraphSAGE and GAT for link prediction. PROBLEM STATEMENT Every team has been assigned one of eight datasets randomly. Each of these datasets represents corresponding seasons from the TV Show, Game of Thrones, where each dataset consists of two CSV files - nodes.csv and edges.csv The former provides the list of characters whereas the latter provides the interactions between them.

The aim is to perform link prediction on this dataset using both traditional and graph machine learning. In this assignment, we will treat link prediction as a binary classification task (i.e. 1 implies that there is a link between the nodes whereas 0 denotes the absence of a link). Subsequently, the methods and thresholds need to be compared and analysed. Any insight drawn from the modelling that matches the storyline should also be stated. REQUIREMENTS

Load the dataset from the CSVs into NetworkX to create an undirected graph.

Perform EDA on the dataset a. Check for isolates, self-loops, etc b. Can be minimal (refer to Lab Evaluation 1 to see what kind of EDA can be done)

Calculate the following measures: a. Betweenness b. PageRank c. Local clustering coefficient These would be the node features in your graph. You are also encouraged to use other node features in addition to these with proper justification as to why they were used, if they help with providing better metrics.

Find communities using Spectral Clustering - Code (for reference only) can be found here. a. Provide hypotheses about how these communities might be getting detected, according to the plot of the season (for example: are they being formed based on the houses the characters belong to?)

Link Prediction using Traditional Methods - Code (for reference only) can be found here. It is recommended that the proximity-based likelihood approach be used, but feel free to use the top-k approach if need be. a. Perform comparison for at least 3 similarity measures - we recommend using Jaccard, Adamic Adar and Preferential Attachment, but you are free to try any others in addition to this. b. Find the best similarity measure along with the optimal threshold for said similarity measure.

Link Prediction using GraphML - Refer to the SEAL paper. a. Load the graph from NetworkX into PyTorch Geometric b. Perform link prediction using i. GCN ii. GraphSAGE iii. GAT c. Compare the three models - use Loss and AUC for comparison (this holds even for traditional link prediction)

Perform a comparison between traditional and GraphML a. What are the metrics? b. Which is performing better? Is there any reason you can think of, as to why this might be happening? c. Any analysis or insights you can draw from this, that may relate to the season’s plot?
