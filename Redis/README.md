## Kubernetes Redis Cluster

Deploy Redis cluster in Kubernetes

![DockerImage-Github](https://github.com/hatamiarash7/Kubernetes-Redis/workflows/DockerImage-Github/badge.svg) ![DockerImage-Dockerhub](https://github.com/hatamiarash7/Kubernetes-Redis/workflows/DockerImage-Dockerhub/badge.svg)
### Introduction
[Redis](https://redis.io) (REmote DIctionary Server) is an open source (BSD licensed), in-memory data structure store, used as a database, cache and message broker. It can store and manipulate high-level data types like lists, maps, sets, and sorted sets. Because Redis can accept keys in a wide range of formats, operations can be executed on the server and reduce the client's workload. Also it holds its database entirely in memory, using the disk only for persistence. Redis is so popular being highly used by tech giants like GitHub, Pinterest, Snapchat, Twitter, StackOverflow, Flickr and many more.

***Why use Redis?**
- It is incredibly fast (written in ANSI C and runs on POSIX systems such as Linux, Mac OS X and Solaris).
- Often ranked the most popular key-value database and the most popular NoSQL database in containers.
- Helps you save cloud database calls using caching solution.
- It can be accessed by applications through its client API library.
- Supported in most of the languages like JavaScript, Java, Go, C, C++, C#, Python, Objective-C, PHP.
- It is open source and stable

***Real examples of use cases**
- some Facebook online games have a very high number of score updates, these operations are trivial using a Redis sorted set, even if there are millions of users and millions of new scores per minute.
- Twitter stores the timeline for all users with a Redis cluster
- Pinterest stores the user follower graphs in a Redis cluster where data is sharded across hundreds of instances
- Github, uses the queueing solution from Redis
