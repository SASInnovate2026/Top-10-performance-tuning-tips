# Tip № 10 Adjust SAS Viya Runtime Engines

The SAS Viya analytic runtime engines are where the real heavy lifting occurs. Monitor their activities and adjust resources as needed for your workloads.

![slide](/img/10.png)

## Links and references

This presentation covers a lot of ground. To help you realize the performance and tuning tips at your site, refer to the following materials for in-depth detail and knowledge.

![sasicon](/img/sas-favicon-16.png) **SAS Communities** (<https://communities.sas.com>)

-   *[Where SAS Viya Relies on Kubernetes for Workload Placement](https://communities.sas.com/t5/SAS-Communities-Library/Where-SAS-Viya-Relies-on-Kubernetes-for-Workload-Placement/ta-p/814780)* <br />SAS Viya relies on Kubernetes to provide a robust environment that is elastic, highly available, extensible, and robust. One way that Kubernetes achieves these goals is through sophisticated workload management controls. By default, SAS Viya takes advantage of these controls in specific ways to ensure the software experience is great. But there's no one-size-fits-all way to deploy SAS Viya, so understanding these controls can be useful to further fine-tune the environment to your site's specific needs.

-   *[How Infrastructure for Kubernetes Helps to Manage SAS Viya Workloads](https://communities.sas.com/t5/SAS-Communities-Library/How-Infrastructure-for-Kubernetes-Helps-to-Manage-SAS-Viya/ta-p/887924)* <br />Understanding how the infrastructure is sized, provisioned, managed, and utilized is part of the foundation to ensuring SAS Viya runs efficiently and effectively.

-   *[Scaling CAS part 1: Add more workers with DAC](https://communities.sas.com/t5/SAS-Communities-Library/Scaling-CAS-part-1-Add-more-workers-with-DAC/ta-p/894790)* <br />The SAS Cloud Analytics Service (CAS) isn't designed to scale elastically (that is, automatically). The starting point is to pick a size and shape for your CAS server deployment and get things running. From there, monitor the environment and adjust the resources for CAS accordingly. In this post, we look at increasing the ***number*** of workers for CAS using the SAS Deployment-as-Code project.

-   *[Scaling CAS part 2: Increase worker size with IAC](https://communities.sas.com/t5/SAS-Communities-Library/Scaling-CAS-part-2-Increase-worker-size-with-IAC/ta-p/894833)* <br />In this post, we look at increasing the ***size*** of workers (more RAM and CPU) for CAS using the SAS Infrastructure-as-Code project.

-   *[Determine how many SAS Viya analytics pods can run on a Kubernetes node](https://communities.sas.com/t5/SAS-Communities-Library/Determine-how-many-SAS-Viya-analytics-pods-can-run-on-a/ta-p/905695)* <br/>Have you ever wondered how many pods of a runtime engine like CAS or Compute can run on a Kubernetes node? How is that determined? What changes can you make? What do we need to consider when trying to trying to match the workload to the available resources?

    We begin with looking at CAS and the unique considerations that a high-performance, in-memory analytics engine requires. We also look at capabilities provided by SAS Workload Management and the impact that has on SAS Compute.  And we wrap up with evaluating the Kubernetes nodes to determine how many pods for runtime engines they can actually support running.

![sasicon](/img/sas-favicon-16.png) **Open source software from SAS Institute Inc.** (<https://github.com/sassoftware>)

-   [SAS Viya Forge](https://viyaforge.sas.com/) <br />SAS Viya Forge is a community-driven repository for documents and tools that help architect, implement and operate your Viya environments. Each piece of content is aimed at ensuring your Viya environment delivers maximum value in the shortest possible time.

-   *[Compare performance of a SAS program between small, medium and large compute contexts](https://gel-innovate.gelenable.sas.com/FANS/main/Session3/05_Bonus.html#19-compare-performance-of-a-sas-program-between-small-medium-and-large-compute-contexts)* <br />After setting up the SPRE with additional resources, it's a good idea to compare performance. This exercise provides a simple methodology to run a test program and evaluate the improvements to execution efficiency.

![sasicon](/img/sas-favicon-16.png) **SAS Documentation** (<https://documentation.sas.com>)

-   *SAS&reg; Viya&reg; Platform Operations* > [System Requirements for the SAS&reg; Viya&reg; Platform](https://go.documentation.sas.com/doc/en/itopscdc/v_074/itopssr/titlepage.htm)
    -   Infrastructure requirements
    -   Hardware and resource requirements
    -   Sizing recommendations
    -   and more

-   *SAS&reg; Viya&reg; Platform Administration* > [Tuning](https://documentation.sas.com/?cdcId=sasadmincdc&cdcVersion=default&docsetId=wrkldmgmt&docsetTarget=titlepage.htm) <br />This guide describes tuning methodologies and considerations for the SAS Viya platform in a Kubernetes environment.

-   *SAS&reg; Viya&reg; Platform Administration* > SAS Cloud Analytic Services > [How To (Tasks)](https://documentation.sas.com/?cdcId=sasadmincdc&cdcVersion=default&docsetId=wrkldmgmt&docsetTarget=titlepage.htm) <br />Instructions for operating the CAS server in Kubernetes, including scaling up/down, converting SMP CAS to MPP, and much more.

-   *SAS&reg; Viya&reg; Platform Administration* > Servers and Services > [Workload Management](https://documentation.sas.com/?cdcId=sasadmincdc&cdcVersion=default&docsetId=wrkldmgmt&docsetTarget=titlepage.htm) <br />SAS Workload Management enhances the performance, resilience, and efficiency of SAS Viya compute services and improves system reliability. It integrates natively with Kubernetes to match workload to compute nodes based on attributes defined in SAS Viya.

![sasicon](/img/sas-favicon-16.png) **SAS Education** (<https://learn.sas.com>)

-   [SAS Architecture and Security Learning Subscription](https://learn.sas.com/totara/program/view.php?id=104) <br />This collection of architecture and security courses are designed for technical architects, administrators, and systems engineers responsible for designing and implementing SAS environments that are secure and fit for purpose.

-   [SAS Deployment Learning Subscription](https://learn.sas.com/totara/program/view.php?id=111) <br />This collection of deployment courses are designed for technical architects, administrators, and systems engineers responsible for designing and deploying SAS technology across supported platforms.

-   [SAS Administration Learning Subscription](https://learn.sas.com/totara/program/view.php?id=73) <br />For SAS administrators responsible for installing and configuring SAS software at their company site, monitoring performance, managing employee access, and troubleshooting issues.

![k8sicon](/img/k8s-favicon-16.png) **Kubernetes Documentation** (<https://kubernetes.io/docs>)

-   Kubernetes > Concepts > Workloads > [Workload Management](https://kubernetes.io/docs/concepts/workloads/controllers/) <br />Kubernetes provides several built-in APIs for declarative management of your workloads and the components of those workloads. These include Deployments, ReplicaSets, StatefulSets, DaemonSets, jobs, and more.

-   Kubernetes > Concepts > Workloads > Pods > [Pod Quality of Service Classes](https://kubernetes.io/docs/concepts/workloads/pods/pod-qos/) <br />Kubernetes assigns a quality of service class to each Pod as a consequence of the resource constraints that you specify for the containers in that Pod. Kubernetes relies on this classification to make decisions about which Pods to evict when there are not enough available resources on a Node.
