# Tip № 3 SPRE Reusable Compute

New pods do not start instantly in Kubernetes - scheduling, pulling container images, and init processes take time. For a pipeline of jobs, this time can add up significantly. Employ Reusable Compute Servers in SAS Viya to keep services ready and waiting for new work, eliminating accumulated wait for startup, and getting results faster.

![slide](/img/03.png)

## Links and references

This presentation covers a lot of ground. To help you realize the performance and tuning tips at your site, refer to the following materials for in-depth detail and knowledge.

![sasicon](/img/sas-favicon-16.png) **SAS Communities** (<https://communities.sas.com>)

- [Improving Concurrency Performance in SAS Viya](https://communities.sas.com/t5/SAS-Communities-Library/Improving-Concurrency-Performance-in-SAS-Viya/ta-p/784542) <br />Out of the box, SAS Viya is configured to ensure it can run without overwhelming the hardware of smaller deployments. One way it does this is to restrict the number of concurrent tasks that are attempted. The scenario here is to improve the user experience in both the SAS Viya user interface as well as the running of compute jobs behinds the scenes. This blog post explains the parameters to adjust and what impact changes to the configuration will make to the system.

- [SAS Viya High Throughput Batch Processing: Part 1 – Reusable Batch Servers]() <br />SAS offers batch capabilities that benefit sites which need extensive batch processing, involving time sensitive, high volumes of SAS jobs of very short duration. These features address some inefficiencies of the default configuration, such as longer turn-around time, excessive resource utilization, potential timeouts and job failures due to sudden surge in number of pod creation.

- [SAS Viya High Throughput Batch Processing: Part 2 – Optimized I/O]() <br />Building on the concurrency improvements described in Part 1, this next post looks at options that provide optimized input and output using file storage.

- [SAS Viya High Throughput Batch Processing: Part 3 – Performance Testing]() <br />To validate the improved configuration, this next post presents performance tests that compare the throughput and total run time of a burst of short-running jobs when run on default batch servers versus high-throughput batch servers.

![sasicon](/img/sas-favicon-16.png) **Open source software from SAS Institute Inc.** (<https://github.com/sassoftware>)

-   tbd

![sasicon](/img/sas-favicon-16.png) **SAS Education** (<https://learn.sas.com>)

-   [SAS Architecture and Security Learning Subscription](https://learn.sas.com/totara/program/view.php?id=104) <br />This collection of architecture and security courses are designed for technical architects, administrators, and systems engineers responsible for designing and implementing SAS environments that are secure and fit for purpose.

-   [SAS Deployment Learning Subscription](https://learn.sas.com/totara/program/view.php?id=111) <br />This collection of deployment courses are designed for technical architects, administrators, and systems engineers responsible for designing and deploying SAS technology across supported platforms.

-   [SAS Administration Learning Subscription](https://learn.sas.com/totara/program/view.php?id=73) <br />For SAS administrators responsible for installing and configuring SAS software at their company site, monitoring performance, managing employee access, and troubleshooting issues.

![sasicon](/img/sas-favicon-16.png) **SAS Documentation** (<https://documentation.sas.com>)

-   *SAS&reg; Viya&reg; Platform Administration* > Servers and Services > Programming Run-Time Servers > SAS Compute: Server, Service, and Contexts > [Reusable Compute Server](https://documentation.sas.com/?cdcId=sasadmincdc&cdcVersion=default&docsetId=calsrvpgm&docsetTarget=p137sodav4z72nn1scp9ccanzpf7.htm#p0erdqd5407a8cn14tt7o84h2g7e) <br />The SAS Compute Server enables clients to submit SAS programs and stored procedures in the form of jobs for processing using the SAS language. Instead of terminating the compute server after the session using it ends, we can enable reusable compute servers that can handle subsequent sessions.

-   *SAS&reg; Viya&reg; Platform Administration* > Servers and Services > Programming Run-Time Servers > [SAS Batch: Server, Service, and Contexts](https://documentation.sas.com/?cdcId=sasadmincdc&cdcVersion=default&docsetId=calsrvpgm&docsetTarget=n0h9w6up3rf2a8n1j68cgh3u74f8.htm) <br />Introduction, refererences, and how to work with the SAS Batch Server aspect of the SAS Programming Runtime Environment.

-   *SAS&reg; Viya&reg; Platform Administration* > Servers and Services > [Workload Management]() <br />SAS Workload Management enhances the performance, resilience, and efficiency of SAS Viya compute services and improves system reliability. It integrates natively with Kubernetes to match workload to compute nodes based on attributes defined in SAS Viya.

![k8sicon](/img/k8s-favicon-16.png) **Kubernetes Documentation** (<https://kubernetes.io/docs>)

-   tbd
