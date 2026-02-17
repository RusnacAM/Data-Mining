# Data-Mining

The dataset to be explored in this project is the Gowalla dataset, found at the [source](https://snap.stanford.edu/data/loc-Gowalla.html).
Gowalla is a location-based social networking website where users built friendship networks and shared their locations through check-ins. The friendship network is represented by an undirected graph, consisting of 196,591 nodes and 950,327 edges. Additionally, it includes 6,442,890 check-ins made by users withing the period Feb 2009 - Oct 2010. Each check-in contains spatial and temporal information.

The track the project follows is Track A: Standard Analysis Project.

// Data cleaning <br>
Before applying any algorithms the validity of the data must be checked. For further analysis it might be useful to know if the friendship graph is connected \ find the connected subgraphs. Secondly, a map of the coordinates can be created. With this it easy to see some outlier check-ins. Secondly, we'd see how large the area of observation is. If it is large enough it might be a good idea to find observation clusters, and in that way we can avoid accounting for the "looping" of coordinates. Furthermore, in order to catch some nonsense data a couple of things can be done: 1. for same location IDs check if the coordinates are similar; 2. For same person check ins that are near in time does it seem that seem like they teleported.
 
// Task Description <br>
In the context of clustering, some of the main tasks would be hierarchical and subspace clustering of user check-in locations. The goal is to provide an analysis on spatial behaviour at multiple scales, for example multiple clusters could represent a street, a neighbourhood, or a city. Based on these scales behaviours can be compared as well, most importantly if different users or communities are similar in distinct subspaces. 

Another point would be hierarchical friend groups, groups at different scales may correspond to one-off meetings, distant friends to close friends and family. Thus, inference of relationships could also be accomplished, the frequency of 2 people checking in at the same time might suggest social ties. Using the same train of thought, the model could even suggest possible friendships if 2 people meeting frequently or occasionally are not already friends according to the graph.

A second focus point would be community detection and sequence segmentation and similarities. The goal is to identify groups of users that are densely connected and analyse if there are mobility patterns based on check in locations. In this case, user check ins are treated as temporal movement sequences. Multiple interesting questions can be explored, such as if the behaviour similarity is based on movement sequence rather than relation and which are the most common routes.

Lastly, a potential focus could be location labeling based on visiting frequency and time, for example, a place that is visited very often by a single person can be labeled as a home location. On the other hand, a place that is primarily visited in the evening by groups of friends might be labeled as night-leisure location. 
