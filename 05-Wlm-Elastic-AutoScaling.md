# Tip № 5 WLM Elastic Autoscaling

SAS Viya Workload Management fully integrates with the Kubernetes Cluster Autoscaler to provide scale from/to zero nodes to help your site save costs in the cloud.

![slide](/img/05.png)

## Links and references

This presentation covers a lot of ground. To help you realize the performance and tuning tips at your site, refer to the following materials for in-depth detail and knowledge.

![sasicon](/img/sas-favicon-16.png) **SAS Communities** (<https://communities.sas.com>)

-  *[Kubernetes autoscaling for SAS Compute workloads might be just a click away](https://communities.sas.com/t5/SAS-Communities-Library/Kubernetes-autoscaling-for-SAS-Compute-workloads-might-be-just-a/ta-p/979213)* <br />Autoscaling as configured by SAS Workload Orchestrator refers to automatically scaling the number of nodes in the Kubernetes cluster to intelligently meet the demands of the current workload. This kind of elastic scalability — that supports scale-from‐ and scale-to-zero nodes — provides a system responsive to different levels of activity while also reducing operation costs for unused resources.

![sasicon](/img/sas-favicon-16.png) **Open source software from SAS Institute Inc.** (<https://github.com/sassoftware>)

-   tbd

![sasicon](/img/sas-favicon-16.png) **SAS Documentation** (<https://documentation.sas.com>)

-   *SAS&reg; Viya&reg; Platform Administration* > Servers and Services > Workload Management > Concepts > [SAS Workload Orchestrator and Kubernetes Cluster Autoscaler Integration](https://documentation.sas.com/?cdcId=sasadmincdc&cdcVersion=default&docsetId=wrkldmgmt&docsetTarget=n1s5vpyfr4sq3zn1i1dp1aotpzka.htm) <br />SAS Workload Orchestrator can use the Kubernetes Cluster Autoscaler to add nodes to node pools (scale up) when a SAS compute pod is pending and there are no resources available on a node on which that pod is allowed to be scheduled. The SAS Workload Orchestrator can also direct workloads so that the Kubernetes Cluster Autoscaler can remove nodes (scale down) when they're no longer needed for the current workload level.

![sasicon](/img/sas-favicon-16.png) **SAS Education** (<https://learn.sas.com>)

-   [SAS Architecture and Security Learning Subscription](https://learn.sas.com/totara/program/view.php?id=104) <br />This collection of architecture and security courses are designed for technical architects, administrators, and systems engineers responsible for designing and implementing SAS environments that are secure and fit for purpose.

-   [SAS Deployment Learning Subscription](https://learn.sas.com/totara/program/view.php?id=111) <br />This collection of deployment courses are designed for technical architects, administrators, and systems engineers responsible for designing and deploying SAS technology across supported platforms.

-   [SAS Administration Learning Subscription](https://learn.sas.com/totara/program/view.php?id=73) <br />For SAS administrators responsible for installing and configuring SAS software at their company site, monitoring performance, managing employee access, and troubleshooting issues.

![k8sicon](/img/k8s-favicon-16.png) **Kubernetes Documentation** (<https://kubernetes.io/docs>)

-   Kubernetes > Concepts > Cluster Administration > [Node Autoscaling](https://kubernetes.io/docs/concepts/cluster-administration/node-autoscaling/) <br />Nodes in your cluster can be autoscaled - dynamically provisioned (scaled up), or consolidated (scaled down) to provide needed capacity while optimizing cost. Autoscaling is performed by Node autoscalers.
