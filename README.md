# Ansible BGPaaS
BGPaaS: Border Gateway Protocol As A Service

Ansible Builder of MP-BGP Router-Reflectors *Stateless* Container Images.

BGP is the network's distributed database, containing entries describing how to reach each machine in the internet. The BGP protocol is very flexible and has been extended multiple times to accommodate new *schemas* (EVPN/Communities/Labels/etc). The distributed aspect comes from the fact that nodes (routers) exchange information and updates over the network, adopting client/server TCP connections. Very often *BGP Servers and Clustering* (Route-Reflectors) are introduced in the BGP topology to simplify  manipulation of entries distributed over the network (Route Leaking/Filtering) and accelerate the distribution of entries over the network (convergence).

The Goals here are:
- **Experiment** and explore new concepts, ideas and use-cases related to Network and PaaS.
- Create **CI/CD** pipeline to run BGP/MP-BGP **ON PaaS**.
- Run **unprivileged** Network containers on PaaS ( Kubernetes + Openshift).
