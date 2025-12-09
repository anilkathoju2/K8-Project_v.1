Kubernetes Project: Deployments & StatefulSets

This project demonstrates how to run stateless and stateful workloads on Kubernetes using Deployments and StatefulSets. It includes example manifests, explanations of key concepts, and instructions for deploying everything to a Kubernetes cluster.

🚀 Overview

Kubernetes offers multiple workload controllers.
This project covers the two most commonly used:

1. Deployments

Best for stateless applications.

Supports rolling updates, rollbacks, scaling.

Pods are interchangeable; identity is not preserved.

Use cases: web servers, REST APIs, stateless microservices.

2. StatefulSets

Best for stateful applications.

Provides stable network IDs and persistent storage.

Pod identity (pod-0, pod-1, …) is preserved.

Use cases: databases (MySQL, PostgreSQL, MongoDB), distributed systems (Kafka, Zookeeper).

Key Differences: Deployment vs StatefulSet
Feature	Deployment	StatefulSet
Pod Identity	No	Yes
Stable Hostnames	No	Yes
Persistent Storage	Optional	Yes (typically required)
Scaling Behavior	Random	Ordered
Rolling Updates	Fast & flexible	Ordered, safer for databases
Best For	Stateless apps	Databases, message queues


📘 Learn More

Kubernetes Deployments:
https://kubernetes.io/docs/concepts/workloads/controllers/deployment/

Kubernetes StatefulSets:
https://kubernetes.io/docs/concepts/workloads/controllers/statefulset/
