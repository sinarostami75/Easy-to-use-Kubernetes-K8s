## Kubernetes Redis Cluster
![zcazcas](https://user-images.githubusercontent.com/62883434/210499256-ca76dccd-0cbe-485c-9f70-8ac3c48740e7.png)

#### Deploy Redis cluster in Kubernetes

![badge (1)](https://user-images.githubusercontent.com/62883434/210497719-5796c850-8f10-4b1b-ba00-8c0e7e54c70d.svg)
![badge](https://user-images.githubusercontent.com/62883434/210497678-51d73d7c-459e-4aa7-8659-93a45219590d.svg)

### Introduction
[Redis](https://redis.io) (REmote DIctionary Server) is an open source (BSD licensed), in-memory data structure store, used as a database, cache and message broker. It can store and manipulate high-level data types like lists, maps, sets, and sorted sets. Because Redis can accept keys in a wide range of formats, operations can be executed on the server and reduce the client's workload. Also it holds its database entirely in memory, using the disk only for persistence. Redis is so popular being highly used by tech giants like GitHub, Pinterest, Snapchat, Twitter, StackOverflow, Flickr and many more.

**Why use Redis?**
- It is incredibly fast (written in ANSI C and runs on POSIX systems such as Linux, Mac OS X and Solaris).
- Often ranked the most popular key-value database and the most popular NoSQL database in containers.
- Helps you save cloud database calls using caching solution.
- It can be accessed by applications through its client API library.
- Supported in most of the languages like JavaScript, Java, Go, C, C++, C#, Python, Objective-C, PHP.
- It is open source and stable

**Real examples of use cases**
- some Facebook online games have a very high number of score updates, these operations are trivial using a Redis sorted set, even if there are millions of users and millions of new scores per minute.
- Twitter stores the timeline for all users with a Redis cluster
- Pinterest stores the user follower graphs in a Redis cluster where data is sharded across hundreds of instances
- Github, uses the queueing solution from Redis
## About Redis Cluster
[Redis Cluster](https://redis.io/topics/cluster-tutorial) is a set of Redis instances, designed for scaling a database by partitioning it, hence making it more resilient. Each member in the cluster, whether a primary or a secondary replica, manages a subset of the hash slot. If a master becomes unreachable then its slave will be promoted to master. In a minimal Redis Cluster made up of 3 master nodes each wigh a single slave node (to allow minimal fail-over), each master node is assigned a hash slot range between 0 and 16,383. Node A will contain hash slots from 0 to 5000, node B from 5001 to 10000, node C from 10001 to 16383. Communication inside the cluster is made via an internal bus, using a gossip protocol in order to propagate information about the cluster or to discover new nodes. 

![Redis-v2-separate-03](https://user-images.githubusercontent.com/62883434/210498297-ac722efc-ab85-4ca9-91a3-99fff2272f08.jpg)

## Quickstart

If you have a running Kubernetes cluster and `kubectl` configured to access it, run the following command to install the operator:

First, you should clone the Redis project, after that, you can create a new directory or folder and copy all config files to that next you can use this command. 

For create namespace use this command or if you have a namespace you should change config file and replace your namespace : 

```bash
kubectl create ns production
```

After Run this command (The first commandment is structure command):

```bash
kubectl apply -f /PATH PROJECT/.
```

Then you can deploy a Redis cluster:

```bash
kubectl apply -f /Redis/.
```
