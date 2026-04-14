# Tip № 1 Better Storage Config

The performance of SAS analytics have long been constrained by disk I/O moreso than CPU or RAM. SAS Viya relies on appropriate Kubernetes storage resources of different kinds depending on the data and access needed. The 3 Starter Storage Classes (3SSC) approach provides a drop-in, no-edit storage configuration that works for any site and cloud provider. Even better, the 3SSC shows how to configure Viya to implement any storage paradigm your site might require.

![slide](/img/01.png)

## Links and references

This presentation covers a lot of ground. To help you realize the performance and tuning tips at your site, refer to the following materials for in-depth detail and knowledge.

![sasicon](/img/sas-favicon-16.png) **SAS Communities** (<https://communities.sas.com>)

-   *[Announcing Project Mountpoint – Guidance to configure storage for SAS Viya](https://communities.sas.com/t5/SAS-Communities-Library/Announcing-Project-Mountpoint-Guidance-to-configure-storage-for/ta-p/984259)* <br />The SAS Viya platform doesn't just need "storage" — it needs the right storage for the job, whether that’s fast, shared, or temporary. We also know site IT teams have strong opinions (and security concerns) about their environments. SAS Viya is designed for storage flexibility through the use of standard Kubernetes conventions.

![sasicon](/img/sas-favicon-16.png) **Open source software from SAS Institute Inc.** (<https://github.com/sassoftware>)

-   [Project Mountpoint](https://github.com/sassoftware/project-mountpoint) (PMP) <br />Gives tools and guidance to streamline configuration of the SAS Viya platform to implement your choice of storage providers in the Kubernetes environment.

-   PMP > [3 Starter Storage Classes](https://github.com/sassoftware/project-mountpoint/tree/main/3SSC-Three-Starter-Storage-Classes) (3SSC) <br />Provides a straightforward, drop-in, no-edit configuration that enables SAS Viya platform operations with three starter storage classes for dynamically-provisioned volumes.

![sasicon](/img/sas-favicon-16.png) **SAS Education** (<https://learn.sas.com>)

-   [SAS Architecture and Security Learning Subscription](https://learn.sas.com/totara/program/view.php?id=104) <br />This collection of architecture and security courses are designed for technical architects, administrators, and systems engineers responsible for designing and implementing SAS environments that are secure and fit for purpose.

-   [SAS Deployment Learning Subscription](https://learn.sas.com/totara/program/view.php?id=111) <br />This collection of deployment courses are designed for technical architects, administrators, and systems engineers responsible for designing and deploying SAS technology across supported platforms.

![sasicon](/img/sas-favicon-16.png) **SAS Documentation** (<https://documentation.sas.com>)

-   *SAS&reg; Viya&reg; Platform Operations* > System Requirements > Hardware and Resource Requirements > [Persistent Storage Volumes, PersistentVolumeClaims, and Storage Classes](https://documentation.sas.com/?cdcId=itopscdc&cdcVersion=default&docsetId=itopssr&docsetTarget=n0ampbltwqgkjkn1j3qogztsbbu0.htm#n1egh9hqndi6lin13w58nozc7vco) <br />Persistent storage volumes with different attributes are required by various SAS Viya platform components.

![k8sicon](/img/k8s-favicon-16.png) **Kubernetes Documentation** (<https://kubernetes.io/docs>)

-   Kubernetes > Storage > [Volumes](https://kubernetes.io/docs/concepts/storage/volumes/) <br />Kubernetes volumes provide a way for containers in a Pod to access and share data via the filesystem. There are different kinds of volume that you can use for different purposes.
