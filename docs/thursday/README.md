- [ ] $\textcolor{orange}{Keynotes (thursday\ October\ 27,\ 2022\ 9:00am\ -\ 10:30am\ EDT)}$
  - [ ] CNCF project and their features overview
    - [ ] Flux 
      - [ ] Open and extensible continuous delivery solution for Kubernetes. Powered by GitOps Toolkit.
      - [ ] it also supports terraform controller
    - [ ] Knative
      - [ ] Knative is a developer-focused serverless application layer which is a great complement to the existing Kubernetes application constructs. Knative consists of two components: an HTTP-triggered autoscaling container runtime called **Knative Serving**, and a CloudEvents-over-HTTP asynchronous routing layer called **Knative Eventing**
    - [ ] Emissary ingress for layer 7
      - [ ] Emissary-Ingress is an open-source Kubernetes-native API Gateway + Layer 7 load balancer + Kubernetes Ingress built on Envoy Proxy.
      - [ ] Emissary-ingress enables its users to:
        - [ ] Manage ingress traffic with load balancing, support for multiple protocols (gRPC and HTTP/2, TCP, and web sockets), and Kubernetes integration
        - [ ] Manage changes to routing with an easy to use declarative policy engine and self-service configuration, via Kubernetes CRDs or annotations
        - [ ] Secure microservices with authentication, rate limiting, and TLS
        - [ ] Ensure high availability with sticky sessions, rate limiting, and circuit breaking
        - [ ] Leverage observability with integrations with Grafana, Prometheus, and Datadog, and comprehensive metrics support
        - [ ] Enable progressive delivery with canary releases
        - [ ] Connect service meshes including Consul, Linkerd, and Istio
        - [ ] Knative serverless integration
    - [ ] Backstage 
      - [ ] Backstage is an open platform for building developer portals
      - [ ] introducing 3rd party security audit and threat model
    - [ ] Cilium
      - [ ] Cilium is a networking, observability, and security solution with an eBPF-based dataplane. It provides a simple flat Layer 3 network with the ability to span multiple clusters in either a native routing or overlay mode. It is L7-protocol aware and can enforce network policies on L3-L7 using an identity based security model that is decoupled from network addressing.
      - [ ] cilium provides sidecar free service mesh
      - [ ] https://github.com/cilium/cilium
      - [ ] 
    - [ ] NATS ( improve usage for k8s)
    - [ ] Cloudevents 
    - [ ] Falco ( runtime security scanning)
    - [ ] Cri-o ( connection monitor)
    - [ ] OpenTelemetry
- [ ] $\textcolor{orange}{Rancher Booth}$
  - [ ] https://github.com/rancher/rancher
  - [ ] https://github.com/rancher/fleet-examples
  - [ ] $\textcolor{green}{Takeaways}$
    - [ ] Rancher is an open sources CNCF project
    - [ ] Rancher can be used to deploy containers and also gives a pretty nice overview to your container (in terms of what you are running and what is failing)
    - [ ] Rancher also gets integrated with fleet which can manage multi-clusters and perform customization such as creating namespaces, updating quotas
- [ ] $\textcolor{orange}{Crossplane Booth}$
  - [ ] https://crossplane.io/
  - [ ] https://crossplane.io/docs/v1.10/concepts/providers.html
  - [ ] $\textcolor{green}{Takeaways}$
    - [ ] Crossplane not only just to manage the EKS/k8s but also EC2 and other infra (AWS and other cloud services)
    - [ ] Crossplane keeps track of the infra and remove if any changes were made manually unless crossplane is paused. this is kind of good and bad 
      - [ ] Good in terms of having one sources of truth instead of each time going thru 100 lines of Terraform Plan and review
      - [ ] Bad in terms of some Cost management tooling
- [ ] $\textcolor{orange}{k3s}$
  - [ ] [Title - Kubernetes On the Edge With K3s For a Smart Metering Use Case](https://kccncna2022.sched.com/event/182GQ/kubernetes-on-the-edge-with-k3s-for-a-smart-metering-use-case-harry-lee-melio-ai?iframe=no&w=100%&sidebar=yes&bg=no)
  - [ ] [presentation](https://static.sched.com/hosted_files/kccncna2022/eb/Kubernetes%20On%20the%20Edge%20With%20K3s%20For%20a%20Smart%20Metering%20Use%20Case.pdf) 
  - [ ] Milio AI is running this on-prem 
  - [ ] K3s - https://k3s.io/ 
    - [ ] choosing this for its flexibility
    - [ ] Support Static Pods with Helm charts
    - [ ] Support single node out of the box
  - [ ] $\textcolor{green}{Takeaways}$
    - [ ] in case we have to run some of the services on-prem in k8s
- [ ] $\textcolor{orange}{CRI-O}$
  - [ ] [Title - CRI-O???s Senior Year](https://kccncna2022.sched.com/event/182Ok/cri-os-senior-year-peter-hunt-urvashi-mohnani-mrunal-patel-red-hat?iframe=no&w=100%&sidebar=yes&bg=no)
  - [ ] Implementation of the k8s Container Runtime interface - Compliant with the Open source
  - [ ] $\textcolor{green}{Takeaways}$
    - [ ] still in early stage but could be a replacement for docker
- [ ] $\textcolor{orange}{CNET Use the CNCF Landscape}$
  - [ ] [Title - How CNET Use the CNCF Landscape To Run High Traffic, Dynamic, Scalable, And Cost-Effective Websites](https://kccncna2022.sched.com/event/182F4/how-cnet-and-friends-use-the-cncf-landscape-to-run-high-traffic-dynamic-scalable-and-cost-effective-websites-corey-mcgalliard-red-ventures?iframe=no&w=100%&sidebar=yes&bg=no)
  - [ ] [presentation](https://static.sched.com/hosted_files/kccncna2022/57/How%20CNET%20%28And%20Friends%29%20Use%20the%20CNCF%20Landscape%20To%20Run%20High%20Traffic%2C%20Dynamic%2C%20Scaleable%2C%20And%20Cost-Effective%20Websites.pdf)
  - [ ] CNET is still on-prem and doesn't have cloud presence at this time
  - [ ] they are also using an internal tool (Deckhand) to create ephemeral environments 
  - [ ] $\textcolor{green}{Takeaways}$
    - [ ] we can adopt some of it we plan to run CCCE application in kubernetes
- [ ] $\textcolor{orange}{Multi-Tenancy For Argo Workflows And Argo CD At Adobe}$
  - [ ] [Title - Multi-Tenancy For Argo Workflows And Argo CD At Adobe](https://kccncna2022.sched.com/event/182Fw/multi-tenancy-for-argo-workflows-and-argo-cd-at-adobe-srinivas-malladi-adobe?iframe=no&w=100%&sidebar=yes&bg=no)
  - [ ] [presentation](https://static.sched.com/hosted_files/kccncna2022/45/KubeCon2022_argo_multi-tenancy.pdf)
  - [ ] Gitops tooling
  - [ ] Git
  - [ ] Argo CD , implemented as k8s Controller
  - [ ] Agro CD, Workflows
    - [ ] Workflow engines
    - [ ] Workflow Tasks
  - [ ] Multi-tenancy in Argo workflows and Argo CD
  - [ ] $\textcolor{green}{Takeaways}$
    - [ ] Agro workflows and Tasks has lots of inbuilt features 
    - [ ] Agro seems a first choice for EKS, as advertized by many companies

- [ ] $\textcolor{orange}{Basics Of Kubernetes}$
  - [ ] [Title - How the Basics Of Kubernetes Auth Scale For Organizations](https://events.linuxfoundation.org/kubecon-cloudnativecon-north-america/program/schedule/)
  - [ ] Basics of Kubernetes Auth Scale For Organizations
  - [ ] Roles have a list of rules , roles lives in namespace
  - [ ] Types of roles
    - [ ] viewer
    - [ ] editor
    - [ ] administrator
  - [ ] ClusterRoles doesn't live in namespace and can list following
    - [ ] namespaces resources
    - [ ] cluster-scoped resources
  - [ ] RoleBinding live in namespace, authorizing resources within namespace
  - [ ] RoleBinding -> Role (within namespace)
  - [ ] ClusterRoleBinding -> ClusterRole
  - [ ] However you can also associate RoleBinding to ClusterRole (this is recommended as you will have fewer roles to manage)
  - [ ] You should run automated integration test to impersonate (kubectl auth can-i --as user_or_svc_account --as-group group)
  - [ ] $\textcolor{green}{Takeaways}$
    - [ ] good understanding in terms of cluster roles
