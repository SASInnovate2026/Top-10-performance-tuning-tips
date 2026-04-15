# Tip № 2 Find Faster SASWORK

SASWORK is scratch space that the SAS programming runtime uses heavily, performing many long, sequential reads and writes of entire tables as part of the analytics process. Ensuring you have the fastest and most cost-effective disk backing SASWORK is an important objective. Learn how to employ multiple SASWORK locations for live, side-by-side performance comparisons without impacting existing configuration so your site can choose the best fit.

![slide](/img/02.png)

## Links and references

This presentation covers a lot of ground. To help you realize the performance and tuning tips at your site, refer to the following materials for in-depth detail and knowledge.

![sasicon](/img/sas-favicon-16.png) **SAS Communities** (<https://communities.sas.com>)

-   *[Announcing Project Mountpoint – Guidance to configure storage for SAS Viya](https://communities.sas.com/t5/SAS-Communities-Library/Announcing-Project-Mountpoint-Guidance-to-configure-storage-for/ta-p/984259)* <br />The SAS Viya platform doesn't just need "storage" — it needs the right storage for the job, whether that’s fast, shared, or temporary. We also know site IT teams have strong opinions (and security concerns) about their environments. SAS Viya is designed for storage flexibility through the use of standard Kubernetes conventions.

-   *[Kubernetes Storage Patterns for SASWORK – part 1](https://communities.sas.com/t5/SAS-Communities-Library/Kubernetes-Storage-Patterns-for-SASWORK-part-1/ta-p/972529)* <br />The SAS Programming Runtime Environment (instantiated as the SAS Compute Server, SAS Connect Server, or SAS Batch Server) is a core workhorse analytics engine for the Viya platform. It relies on disk to hold interim outputs at the ready as it crunches through large volumes of data to complete the job. That scratch space is called SASWORK. We need to address storage performance in terms of raw throughput as well as I/O operations per second to ensure that SAS runtime processing isn’t overly constrained by the storage it’s using for scratch space.

-   *[Kubernetes Storage Patterns for SASWORK – part 2](https://communities.sas.com/t5/SAS-Communities-Library/Kubernetes-Storage-Patterns-for-SASWORK-part-2/ta-p/974761)* <br />Checkpoint-Restart is an optional feature when submitting batch jobs using SAS Workload Management offered as part of the SAS Viya platform running in Kubernetes. This post explains what it takes to set up a shared RWX file system to support these jobs.

-   *[Kubernetes Storage Patterns for SASWORK – part 3](https://communities.sas.com/t5/SAS-Communities-Library/Kubernetes-Storage-Patterns-for-SASWORK-part-3/ta-p/977444)* <br />This post walks through the Kubernetes concepts needed to modify the SPRE pods to implement a new storage provider for the SASWORK volume.

![sasicon](/img/sas-favicon-16.png) **Open source software from SAS Institute Inc.** (<https://github.com/sassoftware>)

-   [Project Mountpoint](https://github.com/sassoftware/project-mountpoint) (PMP) <br />Gives tools and guidance to streamline configuration of the SAS Viya platform to implement your choice of storage providers in the Kubernetes environment.

-   PMP > [Multiple SASWORK Providers](https://github.com/sassoftware/project-mountpoint/tree/main/4-Multiple-SASWORK-Providers) <br />SASWORK is a critical I/O resource to configure properly. For side-by-side testing of different storage technologies to determine the best fit, we can configure the SAS Viya platform to utilize multiple storage providers for SASWORK.

![sasicon](/img/sas-favicon-16.png) **SAS Documentation** (<https://documentation.sas.com>)

-   *SAS&reg; Viya&reg; Platform Operations* > Deployment > Optional Customizations > [Mount Ephemeral Storage for the SAS Programming Run-Time Environment](https://documentation.sas.com/?cdcId=itopscdc&cdcVersion=default&docsetId=dplyml0phy0dkr&docsetTarget=n08u2yg8tdkb4jn18u8zsi6yfv3d.htm#n1rvp1gzc1fqjin12prebnpv2hih) <br />By default the SPRE servers rely on an emptyDir volume for scratch space. However, using the default emptyDir volume is not recommended because SAS programming components can consume large amounts of storage quickly which might inadvertently cause nodes to shut down.

![sasicon](/img/sas-favicon-16.png) **SAS Education** (<https://learn.sas.com>)

-   [SAS Architecture and Security Learning Subscription](https://learn.sas.com/totara/program/view.php?id=104) <br />This collection of architecture and security courses are designed for technical architects, administrators, and systems engineers responsible for designing and implementing SAS environments that are secure and fit for purpose.

-   [SAS Deployment Learning Subscription](https://learn.sas.com/totara/program/view.php?id=111) <br />This collection of deployment courses are designed for technical architects, administrators, and systems engineers responsible for designing and deploying SAS technology across supported platforms.

-   [SAS Administration Learning Subscription](https://learn.sas.com/totara/program/view.php?id=73) <br />For SAS administrators responsible for installing and configuring SAS software at their company site, monitoring performance, managing employee access, and troubleshooting issues.

![k8sicon](/img/k8s-favicon-16.png) **Kubernetes Documentation** (<https://kubernetes.io/docs>)

-   Kubernetes > Storage > [Volumes](https://kubernetes.io/docs/concepts/storage/volumes/) <br />Kubernetes volumes provide a way for containers in a Pod to access and share data via the filesystem. There are different kinds of volume that you can use for different purposes.
