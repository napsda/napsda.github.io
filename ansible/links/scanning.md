# Security Scanning

1. Deploy & run latest scanner on remote nodes
1. Collect report and generate an issue with findings

---
  The [tsunami security scanning project](https://github.com/google/tsunami-security-scanner/blob/master/docs/orchestration.md) is used as the scanning tool. It is usually used to scan running containers from within the same pod in K8s. This project modifies that paradigm by deploying it on a remote VM and running it there. [Tenable](https://www.tenable.com/) was also considered. After scanning we build an issue in Jira (another ticketing system like ServiceNow would be comparable).
---

## Takeaways
1. Use the same scanning tool used for container infrastructure on VMs
1. Integrate with existing chat/issue systems
1. Orchestration handled with ansible and Tower.

  [![DEMO](http://img.youtube.com/vi/YDi-5i2kEfU/0.jpg)](https://youtu.be/YDi-5i2kEfU "Vulnerability Scanning Demo"){:target="_blank"}