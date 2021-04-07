{::options parse_block_html="true" /}
<div class="collapse">
<details><summary markdown="span">Vulnerability Scanning</summary>
<br>

  <span style="color:#0000CD">**Overview:**</span>

  This demonstrating consists of:
  1. Deploy & run latest scanner on remote nodes
  1. Collect report and generate an issue with findings
  
  The [tsunami security scanning project](https://github.com/google/tsunami-security-scanner/blob/master/docs/orchestration.md) is used as the scanning tool. It is usually used to scan running containers from within the same pod in K8s. This project modifies that paradigm by deploying it on a remote VM and running it there. [Tenable](https://www.tenable.com/) was also considered. After scanning we build an issue in Jira (another ticketing system like ServiceNow would be comparable).


  <span style="color:#228B22">**Takeaways:**</span>

  1. Use the same scanning tool used for container infrastructure on VMs
  1. Integrate with existing chat/issue systems
  1. Orchestration handled with ansible and Tower.

  <span style="color:#a50000">**Video Demonstration:**</span>

  [![DEMO](http://img.youtube.com/vi/YDi-5i2kEfU/0.jpg)](https://youtu.be/YDi-5i2kEfU "Vulnerability Scanning Demo"){:target="_blank"}

</details>
</div>
{::options parse_block_html="false" /}
