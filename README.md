Q1-Explain what is a cluster and what is a hadoop cluster.

answer:

1.Cluster is collection of servers and other computing resources which behaves like a single system having  huge processing power and data storage capabilities.Clusters are used mostly in parallel computing applictaions.
2.Hadoop cluster is special type of cluster which consists of software daemons running on commodity hardware capable of handling large amounts of unstructured data in a distributed computing environment.
3. Hadoop cluster has a master-slave architecture.
4.The name node is the master and  it manages file system namespace.It also controls access to files by client.Only one name node exists in every cluster.
5.Data nodes act as slaves and actually serve the read-write requests from clients.Data nodes actually store the blocks and is responsible for creation,deletion and replication of blocks .


Q2-What is meant by a Rack and explain the rack arrangement in a hadoop cluster.

answer:

