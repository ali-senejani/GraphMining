# Exploring_Networkx

This project attempts to explore a public dataset on crime using the Python graph mining library Networkx. 

The aim is to interpret the meaning of results produced by relevant graph mining metrics and to determine whether such results uncover underlying insights.


## DATA

The data which forms the basis of this network was gathered in the 1990s by Rick Rosenfeld and Norm White from police records in the city of St. Louis, USA (Freeman). Rick and Norm began recording names and gender of the victims, suspects, and witnesses of each crime. In total, 829 crimes involving 1,380 persons was documented. From 1,380 persons, 682 were suspects, 557 were victims, 195 were witnesses, and 41 labelled as dual: both suspects and victims of a crime (Freeman). 

The network documents provided by KONECT are based on this data with some modifications (Kunegis). A bipartite relationship was created by having directed edges point from persons to crimes in a document called moreno.out. 

The first column of moreno.out has persons represented as numbers, and in the same way the second column represents crimes, also represented by numbers. For each row, the person on the left column points to the crime in the right column. Moreno.out only contains the edge relationship between two nodes (persons and crimes). Three other documents, each composed of a single column contain the names, gender and role (witness, suspect, victim, dual) involved in a crime. 

The data in the rows of these three documents does not correspond to the data in the rows of moreno.out. For this reason, I was unable to draw a relationship between the number representing a person in moreno.out and the person’s gender, name, or role in the crime recorded in the remaining three documents.  All that could be inferred is that a person node was connected to one or more crimes by means of a directed edge. 


## PROPERTIES OF THE NETWORK

The network generated from moreno.out is an unweighted, directed, bipartite graph containing 2,209 nodes(1380 persons+ 829 crimes) and 1,476 edges (Kunegis).






## WORKS CITED
Freeman, Linton. “Datasets.” http://moreno.ss.uci.edu/data.html#crime.
Kunegis, Jérôme. “Crime.” http://konect.uni-koblenz.de/networks/moreno_crime.

Wikipedia contributors. (2019, November 19). HITS algorithm. In Wikipedia, The Free Encyclopedia. Retrieved 20:11, December 4, 2019, from https://en.wikipedia.org/w/index.php?title=HITS_algorithm&oldid=926895565

Wikipedia contributors. (2019, December 4). PageRank. In Wikipedia, The Free Encyclopedia. Retrieved 20:08, December 4, 2019, from https://en.wikipedia.org/w/index.php?title=PageRank&oldid=929214051

Wikipedia contributors. (2019, November 19). Betweenness centrality. In Wikipedia, The Free Encyclopedia. Retrieved 20:14, December 4, 2019, from https://en.wikipedia.org/w/index.php?title=Betweenness_centrality&oldid=926936096

Wikipedia contributors. (2019, October 10). Closeness centrality. In Wikipedia, The Free Encyclopedia. Retrieved 20:14, December 4, 2019, from https://en.wikipedia.org/w/index.php?title=Closeness_centrality&oldid=920616806


