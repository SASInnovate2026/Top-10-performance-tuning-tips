# Tip № 7 SAS Data Velocity

Working with large volumes of data and achieving the fastest analytic processing might require high-performance data storage.

![slide](/img/07.png)

## Links and references

This presentation covers a lot of ground. To help you realize the performance and tuning tips at your site, refer to the following materials for in-depth detail and knowledge.

![sasicon](/img/sas-favicon-16.png) **SAS Communities** (<https://communities.sas.com>)

-   *[Here Comes SAS&reg; SpeedyStore](https://communities.sas.com/t5/SAS-Communities-Library/Here-Comes-SAS-SpeedyStore/ta-p/968322)* <br />SAS SpeedyStore is a optional product offering that combines SAS’s advanced analytics and AI capabilities seamlessly integrate with SingleStore’s high-performance, cloud-native database, allowing users to perform complex data analysis directly on real-time data stored within SingleStore, resulting in faster insights and improved decision-making without the need for extensive data movement. And it offers advanced database features like point-in-time recovery, audit logging, resource governance, and multi-AZ failover.

-   *[SAS Viya Cloud Analytic Services treats SingleStore differently](https://communities.sas.com/t5/SAS-Communities-Library/Here-Comes-SAS-SpeedyStore/ta-p/968322)* <br />Unlike other data sources that SAS Cloud Analytic Services (CAS) can interoperate with, the partnership that SAS has with SingleStore means that extremely tight integration and efficiencies can be offered.

    > *&#8710; Note this is an older post - most of the content is valid, but improvements to operations since publishing have occurred.*

-   *[Using Grafana dashboards for monitoring SAS SpeedyStore](https://communities.sas.com/t5/SAS-Communities-Library/Using-Grafana-dashboards-for-monitoring-SAS-SpeedyStore/ta-p/973178)* <br />SingleStore have announced that they are depreciating SingleStore DB Studio as their monitoring solution and are moving to using Grafana dashboards. Let's look at implementing the Grafana dashboards for a SAS Viya platform deployment with the SAS SpeedyStore offering, using the SAS Viya Monitoring for Kubernetes project to get started.

![sasicon](/img/sas-favicon-16.png) **Open source software from SAS Institute Inc.** (<https://github.com/sassoftware>)

-   SAS Viya 4 Deployment-as-Code project (DAC) > [SAS Viya Support for SingleStore](https://github.com/sassoftware/viya4-deployment/blob/5078ac75956bcd629fd76cd131ba806e21b7a8bc/docs/user/SingleStore.md) <br />The DAC provides a streamlined approach as an example reference to help with initial deployment of the SAS Viya platform. It includes guidance and examples that include the configurations necessary for SAS SpeedyStore.

![sasicon](/img/sas-favicon-16.png) **SAS Documentation** (<https://documentation.sas.com>)

-   *SAS&reg; Viya&reg; Platform Operations* > Product-Specific Requirements > [SAS SpeedyStore](https://documentation.sas.com/?cdcId=itopscdc&cdcVersion=default&docsetId=itopssr&docsetTarget=n0jq6u1duu7sqnn13cwzecyt475u.htm#n0qs42c42o8jjzn12ib4276fk7pb) <br />The SAS SpeedyStore offering has additional requirements apply to your SAS Viya platform deployment. SAS SpeedyStore includes a data connector for SingleStore, an instance of SingleStore, and additional software components to manage it. SAS SpeedyStore also includes the SAS Embedded Process. The deployment process creates a required service account, sas-singlestore-operator.

-   *SAS&reg; Viya&reg; Platform Administration* > Data > SAS SpeedyStore > [Administration and Configuration Guide](https://documentation.sas.com/?cdcId=sasadmincdc&cdcVersion=default&docsetId=calsinglestore&docsetTarget=titlepage.htm) <br />SAS SpeedyStore (formerly SAS with SingleStore) is an optional software offering that fully integrates a SingleStore database with your SAS Viya platform, providing high-performance parallel data transfer, in-database processing, and other programming efficiencies to operate on large scale analytics tasks.

-   *SAS&reg; Viya&reg; Platform Administration* > Data > SAS SpeedyStore > Deployment > [Adding SAS SpeedyStore to an Existing SAS Viya Platform Deployment](https://documentation.sas.com/?cdcId=sasadmincdc&cdcVersion=v_074&docsetId=calsinglestore&docsetTarget=n1mowsy12qbzq0n1pwws0ettotne.htm) <br />The SAS SpeedyStore product offering can be added to an existing deployment of the SAS Viya platform.

![sasicon](/img/sas-favicon-16.png) **SAS Education** (<https://learn.sas.com>)

-   [SAS Architecture and Security Learning Subscription](https://learn.sas.com/totara/program/view.php?id=104) <br />This collection of architecture and security courses are designed for technical architects, administrators, and systems engineers responsible for designing and implementing SAS environments that are secure and fit for purpose.

-   [SAS&reg; SpeedyStore: Architect and Deploy the SAS&reg; Viya&reg; Platform with SingleStore](https://learn.sas.com/totara/program/view.php?id=73) <br />This course explains key architecture concepts and considerations for the SAS SpeedyStore software offering. Through hands-on exercises, students will be guided step-by-step to architect and deploy the SAS Viya platform with SAS SingleStore in a Microsoft Azure cloud environment.

-   [Engineering and Analyzing Data at Scale with SAS&reg; SpeedyStore](https://learn.sas.com/course/view.php?id=6599) <br />This course is for data and analytics professionals who want to build scalable data pipelines and perform advanced analytics with SAS SpeedyStore.

![s2icon](/img/s2-favicon-16.png) **SingleStore** (<https://singlestore.com>)

-   [SingleStore Documentation](https://docs.singlestore.com/db/v9.0/introduction/singlestore-documentation/) <br />Explore key concepts and features, how SingleStore works, explore the architecture, and more.

-   *[Consolidate Complex Data Workflows Into Fast, Impactful Business Insights](https://www.singlestore.com/blog/consolidate-complex-workflows-with-sas-and-singlestore/)* <br />By embedding SingleStore into SAS Viya, we allow organizations to integrate transactional and analytical data into a comprehensible analytic ready format for downstream AI use cases.  This unified data architecture enables organizations to look at their transactional data and drive analytical models in real-time providing tremendous benefits.
