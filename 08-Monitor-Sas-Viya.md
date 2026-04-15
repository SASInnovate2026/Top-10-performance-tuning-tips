# Tip № 8 Monitor SAS Viya in Kubernetes

There are many software tools we use to deploy, manage, configure, monitor, and troubleshoot SAS Viya in Kubernetes.

![slide](/img/08.png)

## Links and references

This presentation covers a lot of ground. To help you realize the performance and tuning tips at your site, refer to the following materials for in-depth detail and knowledge.

![sasicon](/img/sas-favicon-16.png) **SAS Communities** (<https://communities.sas.com>)

-   *[Observability Solutions for the SAS Viya Platform](https://communities.sas.com/t5/SAS-Communities-Library/Observability-Solutions-for-the-SAS-Viya-Platform/ta-p/900025)* <br />SAS provides administrators with two different observability solutions: SAS Enterprise Session Monitor and SAS Viya Monitoring for Kubernetes. This post explains how they compare and complement each other.

-   *[Comparing Alerting Capabilities of Alertmanager with Grafana](https://communities.sas.com/t5/SAS-Communities-Library/Comparing-Alerting-Capabilities-of-Alertmanager-with-Grafana/ta-p/925286)* <br />Alertmanager and Grafana, both deployed with SAS Viya Monitoring for Kubernetes, possess alerting capabilities. While both serve the purpose of alerting, they have distinct features and approaches that cater to different needs..

-   *[Why you need a log and metric monitoring solution for the SAS Viya platform](https://communities.sas.com/t5/SAS-Communities-Library/Why-you-need-a-log-and-metric-monitoring-solution-for-the-SAS/ta-p/861725)* <br />Troubleshooting problems experienced by SAS Viya in your Kubernetes environment can be challenging if you don't have the necessary metrics and log monitoring in place.

-   *[New Auto-Generation Features for SAS Viya Monitoring](https://communities.sas.com/t5/SAS-Communities-Library/New-Auto-Generation-Features-for-SAS-Viya-Monitoring/ta-p/965723)* <br />SAS Viya Monitoring for Kubernetes provides two features aimed at simplifying deployment: auto-generating Ingress definitions and automatically specifying storage class references. These enhancements reduce the need for manual configuration, making setup easier and more efficient.

-   *[Enhancing Observability: Deploying Pre-Configured Grafana Alerts For Your SAS Viya Platform](https://communities.sas.com/t5/SAS-Communities-Library/Enhancing-Observability-Deploying-Pre-Configured-Grafana-Alerts/ta-p/979484)* <br />SAS Viya Monitoring for Kubernetes offers a set of pre-configured Grafana alerts that can be deployed to enhance monitoring of your SAS Viya platform. These alerts streamline configuration by providing administrators with the option to include SAS Viya-specific alerts right from the moment of deployment. This nicely complements the existing Kubernetes cluster-level alerts deployed with Prometheus to enhance observability and operational readiness.

![sasicon](/img/sas-favicon-16.png) **Open source software from SAS Institute Inc.** (<https://github.com/sassoftware>)

-   *[SAS&reg; Viya&reg; Monitoring for Kubernetes](https://github.com/sassoftware/viya4-monitoring-kubernetes)* (V4M) <br />The SAS Viya Monitoring for Kubernetes project provides scripts and customization options to deploy dashboards for metric monitoring, alerts, and log-message aggregation that target key aspects of the SAS Viya platform.

![sasicon](/img/sas-favicon-16.png) **SAS Documentation** (<https://documentation.sas.com>)

-   *SAS&reg; Viya&reg; Platform Administration* > Configuring your Environment > [Command-Line Interface](https://documentation.sas.com/?cdcId=sasadmincdc&cdcVersion=default&docsetId=calcli&docsetTarget=n01xwtcatlinzrn1gztsglukb34a.htm) (sas-viya CLI) <br />The SAS Viya platform command-line interface (CLI) enables you to interact directly with the SAS Viya platform REST services. Use the CLI to work with the SAS Viya platform programmatically as an alternative to using a graphical user interface (GUI).

-   *SAS&reg; Viya&reg; Platform Administration* > SAS Environment Manager > [User's Guide](https://documentation.sas.com/?cdcId=sasadmincdc&cdcVersion=default&docsetId=evfun&docsetTarget=titlepage.htm) <br />SAS Environment Manager is a web application that enables your site's SAS administrators to examine and manage the various aspects of the SAS Viya platform deployment.

-   *SAS&reg; Enterprise Session Monitor* > [Integrate with SAS Viya Platform on Kubernetes](https://documentation.sas.com/?cdcId=esmoncdc&cdcVersion=default&docsetId=esmonag&docsetTarget=p0dwy8jneeir09n141hcean0hd75.htm) <br />When SAS Enterprise Session Monitor is deployed to a Kubernetes cluster where the SAS Viya platform is running, it automatically detects, categorizes, and monitors SAS Viya processes. Additional configuration can be performed to monitor selected log events.

![sasicon](/img/sas-favicon-16.png) **SAS Education** (<https://learn.sas.com>)

-   [SAS Architecture and Security Learning Subscription](https://learn.sas.com/totara/program/view.php?id=104) <br />This collection of architecture and security courses are designed for technical architects, administrators, and systems engineers responsible for designing and implementing SAS environments that are secure and fit for purpose.

-   [SAS Administration Learning Subscription](https://learn.sas.com/totara/program/view.php?id=73) <br />For SAS administrators responsible for installing and configuring SAS software at their company site, monitoring performance, managing employee access, and troubleshooting issues.

-   [SAS&reg; Viya&reg;: Observability](https://learn.sas.com/totara/program/view.php?id=7784) <br />This workshop provides experience with SAS Viya Monitoring for Kubernetes, SAS Enterprise Session Monitor, and the observability framework supported by SAS for use with Viya on Kubernetes.

&#9463; **Third-party links**

-   Kubernetes Documentation > Reference > [Command line tool (kubectl)](https://kubernetes.io/docs/reference/kubectl/) <br />Kubernetes provides a command line tool for communicating with a Kubernetes cluster's control plane, using the Kubernetes API.

-   [K9s Kubernetes CLI](https://k9scli.io) <br />K9s is a text-based visual interface to interact with your Kubernetes clusters in a terminal window. K9s makes it easier to navigate, observe, and manage your deployed applications in a Kubernetes cluster. K9s continually watches Kubernetes for changes and offers subsequent commands to interact with your observed resources.

-   [Lens IDE for Kubernetes](https://lenshq.io/products/lens-k8s-ide) <br />Lens is a commercial desktop-based integrated development environment (IDE) that provides a unified, visual interface for managing and troubleshooting multiple Kubernetes clusters without needing to rely solely on the command line.

-   [Freelens IDE for Kubernetes](https://freelensapp.github.io) <br />Freelens is a Kubernetes IDE that provides a graphical interface for managing and monitoring Kubernetes clusters. Freelens is maintained by the community.

-   [Grafana](https://grafana.com/oss/grafana/) <br />Collect, correlate, and visualize data with dashboards. Grafana is a visualization and monitoring solution that drives informed decisions, enhances system performance, and streamlines troubleshooting.

-   [Prometheus](https://prometheus.io) <br />Monitor your applications, systems, and services. Instrument, collect, store, and query your metrics for alerting, dashboarding, and other use cases.
