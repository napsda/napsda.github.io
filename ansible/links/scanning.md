## Workflow Overview

1. Deploy & run latest scanner on remote nodes
1. Collect report and generate an issue with findings

The [Tsunami Security Scanning project](https://github.com/google/tsunami-security-scanner/blob/master/docs/orchestration.md) is used as the scanning tool. It is usually used to scan running containers from within the same pod in Kubernetes. This demo shows it is possible to modify that paradigm by deploying the scanner on a remote VM. After scanning we build an issue in Jira 

## Takeaways

1. Use the same scanning tool used for container infrastructure on VMs
1. Integrate with existing chat/issue systems
1. Orchestration handled with ansible and Tower.

Because we are using Ansible it is not difficult to modify this project to use other integrations, for example ServiceNow instead of Jira, or Tenable instead of Tsunami.

## Video Demonstration
[![DEMO](http://img.youtube.com/vi/YDi-5i2kEfU/0.jpg)](https://youtu.be/YDi-5i2kEfU "Vulnerability Scanning Demo"){:target="_blank"}
