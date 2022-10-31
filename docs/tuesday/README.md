- [ ] $\textcolor{orange}{AWS\ containers\ Day}$
  - [ ] AWS containers day was all about CNCF projects and how Amazon is contributing to those and adding features 
  - [ ] Amazon F2 team dedicated to find vulnerabilities
  - [ ] helping to reduce clutter in between gRPC communication between control plane and etcd
  - [ ] helping in improving karpenter 
    - [ ] Karpenter is an open-source node provisioning project built for Kubernetes. Adding Karpenter to a Kubernetes cluster can dramatically improve the efficiency and cost of running workloads on that cluster. Karpenter works by:
      - [ ] **Watching** for pods that the Kubernetes scheduler has marked as unschedulable
      - [ ] **Evaluating** scheduling constraints (resource requests, nodeselectors, affinities,
      - [ ] **tolerations**, and topology spread constraints) requested by the pods
      - [ ] **Provisioning** nodes that meet the requirements of the pods
      - [ ] **Removing** the nodes when the nodes are no longer needed
  - [ ] improving EKS-managed add-ons such as
    - [ ] Amazon VPC CNI plugin for Kubernetes
    - [ ] CoreDNS
    - [ ] kube-proxy
    - [ ] Amazon EBS CSI
  - [ ] [CNI metrics helper to monitor IP addresses](https://docs.aws.amazon.com/eks/latest/userguide/cni-metrics-helper.html)
  - [ ] Using FluentBit with Use_kubelet = True
  - [ ] Enable control plane logging
  - [ ] [Fault injector simulator](https://aws.amazon.com/fis/)
  - [ ] Multi-clusters 
  - [ ] https://github.com/aws/containers-roadmap
  - [ ] https://aws.amazon.com/blogs/containers/
  - [ ] Cdk8s
  - [ ] [Gitops by Flux](https://fluxcd.io/)
  - [ ] Falco , opensource tool for monitoring suspicious activities 
  - [ ] Guard duty and falco are pretty much same
  - [ ] Aws detective is good to understand what and why the issue created
  - [ ] $\textcolor{green}{Takeaways}$
    - [ ] Don’t let security to be an afterthought
    - [ ] give  a try for Flux as open source CICD 
    - [ ] Try using Falco for security of containers
- [ ] CNCF Service mesh solutions
  - [ ] Kubert api ?
  - [ ] BottleRocket OS - https://aws.amazon.com/bottlerocket/