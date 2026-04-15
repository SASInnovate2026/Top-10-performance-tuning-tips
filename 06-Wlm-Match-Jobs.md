# Tip № 6 WLM Can Match Jobs to Hardware

SAS Viya Workload Management provides logical and physical resources to ensure your jobs run where they're supposed to.

![slide](/img/06.png)

## Links and references

This presentation covers a lot of ground. To help you realize the performance and tuning tips at your site, refer to the following materials for in-depth detail and knowledge.

![sasicon](/img/sas-favicon-16.png) **SAS Communities** (<https://communities.sas.com>)

-   *[Kubernetes Storage Patterns for SASWORK – part 3](https://communities.sas.com/t5/SAS-Communities-Library/Kubernetes-Storage-Patterns-for-SASWORK-part-3/ta-p/977444)* <br />This post walks through the Kubernetes concepts needed to modify the SPRE pods to implement a new storage provider for the SASWORK volume.

![sasicon](/img/sas-favicon-16.png) **Open source software from SAS Institute Inc.** (<https://github.com/sassoftware>)

-   [Project Mountpoint](https://github.com/sassoftware/project-mountpoint) (PMP) <br />Gives tools and guidance to streamline configuration of the SAS Viya platform to implement your choice of storage providers in the Kubernetes environment.

-   PMP > [Multiple SASWORK Providers](https://github.com/sassoftware/project-mountpoint/tree/main/4-Multiple-SASWORK-Providers) <br />SASWORK is just one kind of specialized resource your SAS program might need. This exercise is focused on SASWORK, but by extension, it shows how to define new pod templates and SPRE contexts to map the runtime engine to specific infrastructure resources.

![sasicon](/img/sas-favicon-16.png) **SAS Documentation** (<https://documentation.sas.com>)

-   *SAS&reg; Viya&reg; Platform Administration* > Servers and Services > [Workload Management](https://documentation.sas.com/?cdcId=sasadmincdc&cdcVersion=default&docsetId=wrkldmgmt&docsetTarget=titlepage.htm) <br />SAS Workload Management enhances the performance, resilience, and efficiency of SAS Viya compute services and improves system reliability. It integrates natively with Kubernetes to match workload to compute nodes based on attributes defined in SAS Viya.

![sasicon](/img/sas-favicon-16.png) **SAS Education** (<https://learn.sas.com>)

-   [SAS Architecture and Security Learning Subscription](https://learn.sas.com/totara/program/view.php?id=104) <br />This collection of architecture and security courses are designed for technical architects, administrators, and systems engineers responsible for designing and implementing SAS environments that are secure and fit for purpose.

-   [SAS Deployment Learning Subscription](https://learn.sas.com/totara/program/view.php?id=111) <br />This collection of deployment courses are designed for technical architects, administrators, and systems engineers responsible for designing and deploying SAS technology across supported platforms.

-   [SAS Administration Learning Subscription](https://learn.sas.com/totara/program/view.php?id=73) <br />For SAS administrators responsible for installing and configuring SAS software at their company site, monitoring performance, managing employee access, and troubleshooting issues.

![k8sicon](/img/k8s-favicon-16.png) **Kubernetes Documentation** (<https://kubernetes.io/docs>)

-   tbd
