# Tip № 2 Find Faster SASWORK

SASWORK is scratch space that the SAS programming runtime uses heavily, performing many long, sequential reads and writes of entire tables as part of the analytics process. Ensuring you have the fastest and most cost-effective disk backing SASWORK is an important objective. Learn how to employ multiple SASWORK locations for live, side-by-side performance comparisons without impacting existing configuration so your site can choose the best fit.

![slide](/img/02.png)

## Links and references


**SAS Communities** (<https://communities.sas.com>)

-   *[Announcing Project Mountpoint – Guidance to configure storage for SAS Viya](https://communities.sas.com/t5/SAS-Communities-Library/Announcing-Project-Mountpoint-Guidance-to-configure-storage-for/ta-p/984259)* <br />The SAS Viya platform doesn't just need "storage" — it needs the right storage for the job, whether that’s fast, shared, or temporary. We also know site IT teams have strong opinions (and security concerns) about their environments. SAS Viya is designed for storage flexibility through the use of standard Kubernetes conventions.

**Open source software from SAS Institute Inc.** (<https://github.com/sassoftware>)

-   [Project Mountpoint](https://github.com/sassoftware/project-mountpoint) (PMP) <br />Gives tools and guidance to streamline configuration of the SAS Viya platform to implement your choice of storage providers in the Kubernetes environment.

-   PMP > [Multiple SASWORK Providers](https://github.com/sassoftware/project-mountpoint/tree/main/4-Multiple-SASWORK-Providers) <br />SASWORK is a critical I/O resource to configure properly. For side-by-side testing of different storage technologies to determine the best fit, we can configure the SAS Viya platform to utilize multiple storage providers for SASWORK.

**SAS Documentation** (<https://documentation.sas.com>)

-   *SAS&reg; Viya&reg; Platform Operations* > Deployment > Optional Cusomtizations > [Mount Ephemeral Storage for the SAS Programming Run-Time Environment](https://documentation.sas.com/?cdcId=itopscdc&cdcVersion=default&docsetId=dplyml0phy0dkr&docsetTarget=n08u2yg8tdkb4jn18u8zsi6yfv3d.htm#n1rvp1gzc1fqjin12prebnpv2hih) <br />By default the SPRE servers rely on an emptyDir volume for scratch space. However, using the default emptyDir volume is not recommended because SAS programming components can consume large amounts of storage quickly which might inadvertently cause nodes to shut down.

**Kubernetes Documentation** (<https://kubernetes.io/docs>)

-   Kubernetes > Storage > [Volumes](https://kubernetes.io/docs/concepts/storage/volumes/) <br />Kubernetes volumes provide a way for containers in a Pod to access and share data via the filesystem. There are different kinds of volume that you can use for different purposes.
