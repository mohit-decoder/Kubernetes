##Kubernetes Node Affinity and Node Selector Examples

This repository contains three Kubernetes Deployment YAML files that demonstrate different methods to control pod scheduling on specific nodes:

1.  node-selector.yml
2.  preferred-node.yml
3.  required-node.yml

Concept Overview
-   Node Selector: A simple way to constrain a pod to run on nodes with a specific label. It is a hard constraint and is not flexible.

-   Preferred Node Affinity: This is a soft constraint that expresses a preference for the node on which the pod should be scheduled. If the preferred node is not available, the pod can still be scheduled on another node.

-   Required Node Affinity: This is a hard constraint that forces the pod to be scheduled only on nodes that match the specified criteria. If no matching nodes are available, the pod will not be scheduled.
