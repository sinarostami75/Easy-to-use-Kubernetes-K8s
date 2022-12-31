# Kubernetes (K8s)


![Kubernetes-Logo-PNG1](https://user-images.githubusercontent.com/62883434/210126977-723d7cd8-b6e7-4627-b086-aa21713888b7.png)

Kubernetes is an open-source container orchestration system for automating software deployment, scaling, and management.
Kubernetes, also known as K8s, is an open source system for managing containerized applications across multiple hosts. It provides basic mechanisms for deployment, maintenance, and scaling of applications.

Kubernetes builds upon a decade and a half of experience at Google running production workloads at scale using a system called Borg, combined with best-of-breed ideas and practices from the community.

Kubernetes is hosted by the Cloud Native Computing Foundation (CNCF). If your company wants to help shape the evolution of technologies that are container-packaged, dynamically scheduled, and microservices-oriented, consider joining the CNCF. For details about who's involved and how Kubernetes plays a role, read the CNCF announcement.

#To start using K8s
See our documentation on kubernetes.io.

Try our interactive tutorial.

Take a free course on Scalable Microservices with Kubernetes.

To use Kubernetes code as a library in other applications, see the list of published components. Use of the k8s.io/kubernetes module or k8s.io/kubernetes/... packages as libraries is not supported.

To start developing K8s
The community repository hosts all information about building Kubernetes from source, how to contribute code and documentation, who to contact about what, etc.

If you want to build Kubernetes right away there are two options:

You have a working Go environment.
mkdir -p $GOPATH/src/k8s.io
cd $GOPATH/src/k8s.io
git clone https://github.com/kubernetes/kubernetes
cd kubernetes
make
You have a working Docker environment.
git clone https://github.com/kubernetes/kubernetes
cd kubernetes
make quick-release
For the full story, head over to the developer's documentation.

#Support
If you need support, start with the troubleshooting guide, and work your way through the process that we've outlined.

That said, if you have questions, reach out to us one way or another.

#Community Meetings
The Calendar has the list of all the meetings in Kubernetes community in a single location.

#Adopters
The User Case Studies website has real-world use cases of organizations across industries that are deploying/migrating to Kubernetes.

#Governance
Kubernetes project is governed by a framework of principles, values, policies and processes to help our community and constituents towards our shared goals.

The Kubernetes Community is the launching point for learning about how we organize ourselves.

The Kubernetes Steering community repo is used by the Kubernetes Steering Committee, which oversees governance of the Kubernetes project.

#Roadmap
The Kubernetes Enhancements repo provides information about Kubernetes releases, as well as feature tracking and backlogs.
