---
title: "multicluster"
url: "https://coredns.io/explugins/multicluster/"
date: "2023-03-03"
feed_url: "https://coredns.io/explugins/index.xml"
---
Description The multicluster plugin implements the Kubernetes DNS-Based Multicluster Service Discovery Specification. Syntax multicluster [ZONES...] { kubeconfig KUBECONFIG [CONTEXT] noendpoints fallthrough [ZONES...] } kubeconfig KUBECONFIG [CONTEXT] authenticates the connection to a remote k8s cluster using a kubeconfig file. [CONTEXT] is optional, if not set, then the current context specified in kubeconfig will be used.
