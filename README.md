Q1-Explain what is a cluster and what is a hadoop cluster.

answer:

1.Cluster is collection of servers and other computing resources which behaves like a single system having  huge processing power and data storage capabilities.Clusters are used mostly in parallel computing applictaions.
2.Hadoop cluster is special type of cluster which consists of software daemons running on commodity hardware capable of handling large amounts of unstructured data in a distributed computing environment.
3. Hadoop cluster has a master-slave architecture.
4.The name node is the master and  it manages file system namespace.It also controls access to files by client.Only one name node exists in every cluster.
5.Data nodes act as slaves and actually serve the read-write requests from clients.Data nodes actually store the blocks and is responsible for creation,deletion and replication of blocks .


Q2-What is meant by a Rack and explain the rack arrangement in a hadoop cluster.

answer:

Rack:
A collection nodes physically stored close togather and connected to a same network switch is called Rack.

Rack arrangement in Hadoop:

1.In large clusters of hadoop ,in order to improve network traffic while accessing files, name node chooses data nodes which are on the same rack or a nearby rack to read/write request.
2.Name node achieves this rack information by maintaining rack ids of each data node.This concept of choosing closer data nodes based on racks information is called rack awareness in hadoop.
3.A default hadoop installation assumes that all the nodes belong to the same rack.
4.A simple policy is to place replicas across racks.This prevents loss of data when an entire rack fails and allows to make use of bandwidth from multiple racks when reading  a file.
5.on multiple racks cluster, block replications are maintained with a policy of no more than one replica is placed on one node and no more than 2 replicas are placed in the same rack with a constraint that number of racks used for block replication should always be less than total number of block replicas.

