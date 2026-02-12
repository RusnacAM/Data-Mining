# Data-Mining

The dataset to be explored in this project is the Gowalla dataset, found at the [source](https://snap.stanford.edu/data/loc-Gowalla.html).
Gowalla is a location based social networking website where users have a friendship network built and they can share their location with said network by checking-in. The friendship network is represented by an undirected graph, consisting of 196,591 nodes and 950,327 edges. Each user represents a node, an edge between two users is a relationship. To supplement this, another file is provided with time and location information of check-ins made by users. In total, 6,442,890 check-ins were made by users between a almost 2 year period between feb 2009 - oct 2010.

// Data cleaning <br>
Before applying any algorithms the validity of the data must be checked. For further analysis it might be useful to know if the frienship graph is connected \ find the connected subgraphs. Secondly, it must be checked if the "looping" of coordinates needs to be accounted for i.e. is the area of our observations large enough. Furthermore, in order to catch some nonsense data a couple of things can be done: 1. for same location IDs check if the coordiantes are similar; 2. For same person check ins that are near in time does it seem that seem like they teleported.
 
// Clustering <br>
In the context of clustering, the main task on this dataset would be hirearchical and subspace clustering of user check-in locations. The goal is to provide an analysis on spatial behaviour at multiple scales, for example multiple clusters could represent a street, a neighbourhood, thus patterns of behaviour can e analysed relative to different granularities. Based on these scales behvaiours can be compared as well, most importantly if different users or communities are similar in distinct subspaces.

// Graph mining, pattern mining <br>
The task proposed in this project is community detection and sequence segmentation and similarities. The goal identify groups of users that are densely connected and analyse if there are mobility patterns based on check in locations. This problem could also be analysed in the context of pattern mining - sequence segmentation and similarities. In this case, user check ins are treated as temporal movement sequences, thus patterns and routines can be identified. Multiple interesting questions can thus be explored, such as if the behaviour similarity is based on movement sequence rather than relation and which are the most common routes.
