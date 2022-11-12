## ServiceMesh

**Application networking day with Istio, Ambient Mesh, Cilio**

Modern applications are orchestrated as collections of microservices and each of them meant to perform discrete set of functions. Service mesh allows us to establish below list of things instead of adding to our code,
  * traffic management
  * Security
  * Observability

#### What is Istio? ####
Istio is an open source service mesh helps in establishing the connectivity onto existing distributed applications. Its powerful control plane brings vital features, including:

  * Secure service-to-service communication
  * Automatic load balancing.
  * Fine-grained control of traffic behavior.
  * A pluggable policy layer and configuration API.
  * Automatic metrics, logs, and traces.

#### Ambient Mesh ####
Now, let's talk about the challenges with Istio where it is deployed as a sidecar. Although sidecars have significant advantages over refactoring applications, they do not provide a perfect separation between applications and the Istio data plane.

Ambient mesh uses a shared agent, running on each node in the Kubernetes cluster. This agent is a zero-trust tunnel (or ztunnel), and its primary responsibility is to securely connect and authenticate elements within the mesh.

<img width="715" alt="image" src="https://user-images.githubusercontent.com/16527158/201456912-e77ac71b-38ec-48cc-b7db-202cf5eff93b.png">

<img width="568" alt="image" src="https://user-images.githubusercontent.com/16527158/201456943-e08e2d0c-d9cf-4ac4-862a-6de1ac7c5149.png">



<img width="481" alt="image" src="https://user-images.githubusercontent.com/16527158/201453279-edd72df3-532c-4989-9a43-774c97e4f0d5.png">
