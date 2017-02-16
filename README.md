1.  Explain what is a cluster and what is a hadoop cluster?

Cluster:
Clustering can be considered the most important unsupervised learning problem; so, as every other problem of this kind, it deals with finding a structure in a collection of unlabeled data.
A loose definition of clustering could be “the process of organizing objects into groups whose members are similar in some way”.
A cluster is therefore a collection of objects which are “similar” between them and are “dissimilar” to the objects belonging to other clusters.

The Goals of Clustering:

So, the goal of clustering is to determine the intrinsic grouping in a set of unlabeled data. But how to decide what constitutes a good clustering? It can be shown that there is no absolute “best” criterion which would be independent of the final aim of the clustering. Consequently, it is the user which must supply this criterion, in such a way that the result of the clustering will suit their needs.
For instance, we could be interested in finding representatives for homogeneous groups (data reduction), in finding “natural clusters” and describe their unknown properties (“natural” data types), in finding useful and suitable groupings (“useful” data classes) or in finding unusual data objects (outlier detection).



Hadoop Cluster:
Normally any set of loosely connected or tightly connected computers that work together as a single system is called Cluster. In simple words, a computer cluster used for Hadoop is called Hadoop Cluster. 

Hadoop cluster is a special type of computational cluster designed for storing and analyzing vast amount of unstructured data in a distributed computing environment. These clusters run on low cost commodity computers. 
Hadoop clusters are often referred to as "shared nothing" systems because the only thing that is shared between nodes is the network that connects them. 
Large Hadoop Clusters are arranged in several racks. Network traffic between different nodes in the same rack is much more desirable than network traffic across the racks. 

Hadoop cluster has 3 components:
- Client
- Master
- Slave

2. What is meant by a Rack and explain the rack arrangement in a hadoop cluster?

Rack:
 	A rack server, also called a rack-mounted server, is a computer dedicated to use as a server and designed to be installed in a framework called a rack. The rack contains multiple mounting slots called bays, each designed to hold a hardware unit secured in place with screws. 
A rack server has a low-profile enclosure, in contrast to a tower server, which is built into an upright, standalone cabinet.

A single rack can contain multiple servers stacked one above the other, consolidating network resources and minimizing the required floor space. The rack server configuration also simplifies cabling among network components. 
In an equipment rack filled with servers, a special cooling system is necessary to prevent excessive heat buildup that would otherwise occur when 
many power-dissipating components are confined in a small space.

Rack Awareness:

	Rack awareness is having the knowledge of Cluster topology or more specifically how the different data nodes are distributed across the racks of a Hadoop cluster. 
The importance of this knowledge relies on this assumption that collocated data nodes inside a specific rack will have more bandwidth and less latency whereas two data nodes 
in separate racks will have comparatively less bandwidth and higher latency.

The main purpose of Rack awareness is:

- Increasing the availability of data block
- Better cluster performance

You can make a Hadoop cluster rack aware by using a script that enables the master node to map the network topology of the cluster. It does so using the properties topology.script.file.name or net.topology.script.file.name, available in the core-site.xml configuration file.
