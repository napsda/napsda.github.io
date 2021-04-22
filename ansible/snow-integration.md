{::options parse_block_html="true" /}
<div class="collapse">
<details><summary markdown="span">Closed Loop Incident Management</summary>
<br>

  <span style="color:#0000CD">**Overview:**</span>

  1. Initiate Compliance Check via Slack
  2. Ansible detects out of compliance and opens ticket in ServiceNow
  3. ServiceNow business logic instructs back to Ansible to remediate
  4. Ansible completes remediation and marks ServiceNow ticket as resolved and closes it out
  5. Slack notifies requestor of updates

  <span style="color:#228B22">**Takeaways:**</span>

  - Ansible is the **`glue`** by being able to integrate with almost any system to enhance business processes and operations
  - View Ansible as an Enterprise wide tool vs. point OS automation
  - Machine to machine communication is the key to automation at scale

  <span style="color:#a50000">**Video Demonstration:**</span>

  [![DEMO](http://img.youtube.com/vi/Ye-OYPHH6es /0.jpg)](http://www.youtube.com/watch?v=Ye-OYPHH6es "Closed Loop Incident Management"){:target="_blank"}

</details>
</div>
{::options parse_block_html="false" /}