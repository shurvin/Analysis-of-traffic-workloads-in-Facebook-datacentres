## Analysis-of-traffic-workloads-in-Facebook-datacentres
### Background introduction
The *Facebook datacenter fabric* now supports more than 2.6 billion people using real-time applications and rapidly scaling (2019). Facebook traffic is accompanied by an expansion of the network structure (search, ad selection, and event logging), and traffic workload analysis in FB data centers is particularly needed. The input to the system or the load applied to the system is called the workload. For databases, workloads are database requests and commands issued by clients. Requests: Workload imposed. Latency: the response time of the application.
Objective: Study the statistical characteristics of a publicly accessible workload from Facebook datacenters and subsequently develop a model which faithfully capture those characteristics. Such as traffic characteristics, patterns are present and workload types.
Method: For the data transmission problem with large amount of data, there are two kinds of methods. One method is to transmit only the updated part of the interface when the interface is refreshed, the other is to use a compression method inside each instruction set.
###  Characteristics of publicly accessible workloads in Facebook data centers:
1. Average server or resource busy time of the corresponding proportional formula is: Non-free time = Busy time/ Observation period
2. For workload scalability studies, regression analysis is performed here to determine the value of the Amdahl coefficient (see the code file for details). Investigate how performance changes as the load scales.
3. Get some data support based on Inside the Social Network’s (Datacenter) Network.
The web tier is generally stateless and easy to scale horizontally. Since any server can handle any request, various traffic routing strategies can be used: on and off mode, rapid growth in usage and instantaneous pump mode.
Hadoop clusters perform offline analysis such as data mining.
Traffic in back-end database clusters is the most uniform, divided almost evenly amongst nodes within the cluster, the same datacenter, and worldwide.
Hadoop server communicates with 1.5% of the other servers in the cluster—spread across 95% of the racks though only 17% of the racks receive over 80% of the server’s traffic.
4.The rack-to-rack traffic matrix of pods inside one of the new Fabric datacenters over a day-long period.
5.Data center contains multiple clusters (Datacenters can grow to a certain size until their sheer size becomes a liability with no additional scale advantage and thus they are broken up into clusters.), storage pools, and networks. A cluster consists of multiple servers with RHVH installed, virtual machines are created on the cluster, and a virtual machine is allowed to run on any server in the cluster.

