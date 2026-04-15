# Tip № 4 SAS Code Analyzer (SCAPROC)

Use the SCAPROC procedure to scan your existing monolithic SAS program code to identify how it can be refactored to submit smaller jobs that run concurrently in less time, better utilizing your compute resources, and returning results faster.

![slide](/img/04.png)

## Links and references

This presentation covers a lot of ground. To help you realize the performance and tuning tips at your site, refer to the following materials for in-depth detail and knowledge.

![sasicon](/img/sas-favicon-16.png) **SAS Communities** (<https://communities.sas.com>)

- *[SCAPROC: generating parallel code for SAS Viya](https://communities.sas.com/t5/SAS-Communities-Library/SCAPROC-Generating-Parallel-Code-for-SAS-Viya/ta-p/986310)* <br />The SAS Code Analyzer procedure examines your SAS program code, idenitifies the dependencies, and outputs an updated program that will automatically spawn parallel jobs that run concurrently to reduce your overall execution time.

![sasicon](/img/sas-favicon-16.png) **Open source software from SAS Institute Inc.** (<https://github.com/sassoftware>)

-   [Project Mountpoint](https://github.com/sassoftware/project-mountpoint) (PMP) <br />Gives tools and guidance to streamline configuration of the SAS Viya platform to implement your choice of storage providers in the Kubernetes environment.

-   PMP > [Additional RWX volumes for SPRE](https://github.com/sassoftware/project-mountpoint/tree/main/6-Addtl-RWX-Volume-for-SPRE) <br />Out of the box, the SPRE pods - that is, SAS Batch, SAS Compute, and SAS Connect servers - only define the minimum storage volumes for initial operations. For parallel jobs that might refer to the same interim data outputs, "gridwork" is a shared RWX volume that jobs can use to store their program, output, and job information.

![sasicon](/img/sas-favicon-16.png) **SAS Documentation** (<https://documentation.sas.com>)

-   *SAS&reg; Viya&reg; Platform Programming Documentation* > SAS Language Reference > Base SAS Procedures > [SCAPROC Procedure](https://documentation.sas.com/?cdcId=pgmsascdc&cdcVersion=default&docsetId=proc&docsetTarget=p0sf63lx4fs2m5n14qv1bn8p863v.htm) <br />The SCAPROC procedure implements the SAS Code Analyzer, which captures information about input, output, and the use of macro symbols from a SAS job while it is running. The SAS Code Analyzer can write this information and the information that is in the original SAS file to a file that you specify. The SCAPROC procedure can also generate a grid-enabled job that can concurrently run independent pieces of the job.

-   *SAS&reg; Viya&reg; Platform Administration* > Servers and Services > [Workload Management](https://documentation.sas.com/?cdcId=sasadmincdc&cdcVersion=default&docsetId=wrkldmgmt&docsetTarget=titlepage.htm) <br />SAS Workload Management enhances the performance, resilience, and efficiency of SAS Viya compute services and improves system reliability. It integrates natively with Kubernetes to match workload to compute nodes based on attributes defined in SAS Viya.

![sasicon](/img/sas-favicon-16.png) **SAS Education** (<https://learn.sas.com>)

-   [SAS Architecture and Security Learning Subscription](https://learn.sas.com/totara/program/view.php?id=104) <br />This collection of architecture and security courses are designed for technical architects, administrators, and systems engineers responsible for designing and implementing SAS environments that are secure and fit for purpose.

-   [SAS Deployment Learning Subscription](https://learn.sas.com/totara/program/view.php?id=111) <br />This collection of deployment courses are designed for technical architects, administrators, and systems engineers responsible for designing and deploying SAS technology across supported platforms.

-   [SAS Administration Learning Subscription](https://learn.sas.com/totara/program/view.php?id=73) <br />For SAS administrators responsible for installing and configuring SAS software at their company site, monitoring performance, managing employee access, and troubleshooting issues.

-   [Architecture and Administration for SAS&reg; Workload Management on SAS&reg; Viya&reg;](https://learn.sas.com/course/view.php?id=6485) <br />The course examines SAS Workload Orchestrator software and outlines general concepts and usage scenarios, architecture and deployment considerations, and administration and monitoring functions.

![k8sicon](/img/k8s-favicon-16.png) **Kubernetes Documentation** (<https://kubernetes.io/docs>)

-   Kubernetes > Concepts > [Workloads](https://kubernetes.io/docs/concepts/workloads/) <br />A workload is an application running on Kubernetes. Whether your workload is a single component or several that work together, on Kubernetes you run it inside a set of pods. In Kubernetes, a Pod represents a set of one or more running containers on your cluster. Kubernetes provides resources to make sure the right kind of pods are running to match the desired state.
