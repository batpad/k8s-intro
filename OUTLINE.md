### A Brief History of Deploying Things

 - The good ol' days: ssh into a server, install all the things.
 - Tools to manage installs and operations across multiple servers: chef, puppet, etc. - "infrastructure as code".
 - Isolating dependencies between applications: Virtual Machines
 - Horizontal scaling: separation of layers
 - The rise of containers (lxc -> Docker)
 - Changing roles: Sysadmin -> Devops
 - A modern deployment: infrastructure defined as code, scalable across physical hardware, secure, with monitoring, logging.
 - Various cloud and proprietary solutions: Docker Swarm, AWS ECS + CloudFormation.
 - Open Source / Cross-Cloud / Can be run on off-the-shelf hardware: The rise of Kubernetes.

 ### Kubernetes Fundamentals

  - A "cluster": the control pane / master node, that maintains `etcd`, a distributed key value store maintaining the "state" of the cluster.
  - Specify Kubernetes resources as YAML and apply them onto the cluster, modifying its state.
  - Control pane reads changes to the desired state of the cluster and applies changes by assigning workloads onto worker nodes, via a Scheduler.
  - Basic anatomy of a Kubernetes YAML file
  - Basic Resource Types: Pods, Deployments, Services, Storage, Stateful Sets, Jobs, CronJobs.
  - Passing parameters / templating YAML configuration / package management for Kubernetes: Helm (+alternatives like Kubeflow)

### Using (and pronouncing) kubectl

 - Swiss army knife to interact with cluster
 - Inspect running workloads, describe any resource
 - Debugging: logs, monitoring, ssh-ing into containers, port-forwarding to localhost

### Code Walkthrough and Practical Examples

 - Putting together the toolchain: Helm + Chartpress
 - Using Github Actions for CI: Build Images + Deploy OR publish Helm Charts
 - Osm-seed quick walkthrough
 - Lulc-Infra quick walkthrough
 - Some concepts: Custom Annotations, Auto-Scaling, Persistent Volumes + StatefulSets, Node Selectors
 - Configuring routing and HTTPS: Ingress and Ingress Controllers

### Setting up cluster

 - Setups on different cloud providers: AKS, EKS, GKE, local



 
