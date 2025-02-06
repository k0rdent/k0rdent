![Light/Dark Mode Image](https://github.com/k0rdent/k0rdent/img/k0rdent-logo-horizontal-inverted-dark-mode.png#gh-dark-mode-only)
![Light/Dark Mode Image](https://github.com/k0rdent/k0rdent/img/k0rdent-logo-horizontal-light-mode.png#gh-light-mode-only)

<h1 align="center" weight='300' >Deploy and Manage Kubernetes at scale</h1>
<h3 align="center" weight='300' >Visit <a href="https://docs.k0rdent.io" target="_blank">k0rdent docs</a> for the full documentation,
examples and guides.</h3>
<div align="center">




[![slack](https://img.shields.io/badge/slack-k0rdent-brightgreen.svg?logo=slack)](https://cloud-native.slack.com/archives/C08A63Q4NCD) [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://github.com/k0rdent/k0rdent/blob/main/LICENSE) [![X/Twitter][x-badge]][x-link]



[x-badge]:https://img.shields.io/twitter/follow/k0rdent?logo=x&style=flat
[x-link]:https://x.com/k0rdent

</div>

k0rdent is dedicated to establishing a standardized and efficient approach to deploying and managing Kubernetes clusters at scale. It functions as a "super control plane," orchestrating and managing multiple Kubernetes control planes seamlessly. Alternatively, k0rdent can be viewed as a powerful open-source platform tailored for Platform Engineering, offering tools to streamline workflows and enhance operational efficiency.

If you are building an Internal Developer Platform (IDP), require centralized management of Kubernetes clusters, or wish to create Golden Paths for consistent development practices, k0rdent is an ideal solution. It simplifies complex operations, enabling platform engineers to focus on delivering value.

Whether managing Kubernetes clusters on-premises, in the cloud, or across hybrid environments, k0rdent ensures consistency and reliability. With comprehensive lifecycle management capabilities—including provisioning, configuration, and maintenance—k0rdent provides a repeatable, secure, and centralized method to oversee Kubernetes clusters effectively.

#### k0rdent Components
The main components of k0rdent include:

- **k0rdent Cluster Manager (kcm)**

Deployment and life-cycle management of Kubernetes clusters, including configuration, updates, and other CRUD operations.

- **k0rdent State Manager (ksm)**

Installation and life-cycle management of beach-head services, policy, Kubernetes API configurations and more.

- **k0rdent Observability and FinOps (kof)**

Cluster and beach-head services monitoring, events and log management.


<h1 id="installation">🛠️ Quickstart & Installation</h1>

The QuickStart shows and briefly explains the hows, whys, and wherefores of manually setting up k0rdent for use. Once built and validated, the QuickStart setup can be leveraged to begin an expanding sequence of demos that let you explore k0rdent's many features.

Get started with k0rdent in just a few steps by referring to the [Quickstart Guide](https://docs.k0rdent.io/latest/guide-to-quickstarts/)

The process of installing k0rdent is straightforward, and involves the following steps:

- Create a Kubernetes cluster to act as the management cluster
- Install k0rdent into the management cluster
- Add the necessary credentials and templates to work with the providers in your infrastructure.

Here is the full [Administrator's Guide To Install k0rdent](https://docs.k0rdent.io/latest/admin-installation/).

  
<h1 id="architecture">📐 Architecture</h1>

The k0rdent architecture follows a declarative approach to cluster management using the principles of the Kubernetes Cluster API (CAPI), where you define the state you want using YAML and CAPI ensures you get it. For example, if you wanted to create a new cluster, you’d define that cluster just as you’d define a Pod or other Kubernetes object, then apply the YAML file to the Management Cluster, which acts as the heart of the system. 

The Management Cluster can orchestrate the provisioning and lifecycle of multiple child clusters, keeping you from having to directly interact with individual infrastructure providers. This way, you can define your cluster in one cloud environment, such as AWS, then re-use that definition in another cloud, like Azure, largely unchanged.

<p align="center">
  <img alt="k0rdent architecture" img src="/img/k0rdent_architecture.png" height="450px">
</p>

The k0rdent architecture comprises the following components:
- Cluster Management: Tools and controllers for defining, provisioning, and managing clusters.
- State Management: Controllers and systems for monitoring, updating, and managing the state of child clusters and their workloads.
- Infrastructure Providers: Services and APIs responsible for provisioning resources such as virtual machines, networking, and storage for clusters.
- Templates: Templates that can be used to define and create managed child clusters or the workloads that run on them.



<h1 id="community">👋 Community</h1>


We welcome contributions from the wider community! Read this [guide](https://github.com/k0rdent/k0rdent/blob/main/CONTRIBUTING.md) to get started, and join our thriving community on [Slack](https://cloud-native.slack.com/archives/C08A63Q4NCD).

🌟 [Leave us a star](https://github.com/k0rdent/k0rdent), it helps the project to get discovered by others and keeps us motivated to build awesome open-source tools! 🌟

<h1 id="contributing">👥 Contributing</h1>

To learn about how to contribute to k0rdent, see our [contributing documentation](https://github.com/k0rdent/k0rdent/blob/main/CONTRIBUTING.md).

k0rdent contributors must follow the [k0rdent Code of Conduct](https://github.com/k0rdent/community/blob/main/CODE_OF_CONDUCT.md).

To learn about k0rdent governance, see our [community governance document](https://github.com/k0rdent/community/blob/main/GOVERNANCE.md).

<h1 id="license">📃 License</h1>

Apache License 2.0, see [LICENSE](https://github.com/k0rdent/k0rdent/blob/main/LICENSE).


<h1 id="project resources">💼 Project Resources</h1>

- [k0rdent Community Details](https://github.com/k0rdent/community)
- Join the [#k0rdent](https://cloud-native.slack.com/archives/C08A63Q4NCD) community slack channel on the [CNCF](https://slack.cncf.io) Slack space.
- k0rdent GitHub:  https://github.com/k0rdent
-  k0rdent docs: https://k0rdent.github.io/docs/
