{::options parse_block_html="true" /}
<div class="collapse">
<details><summary markdown="span">Multi-Cloud Provisioning</summary>
<br>

  <span style="color:#0000CD">**Overview:**</span>

  The multi-cloud demo (workflow) consists of:
  1. Provision VMs in (1) Azure and (2) AWS
  2. In AWS configure an Apache server, in Azure an IIS server.
  3. Post in slack channel that multi-cloud workflow has finished.
  4. If any of the process fails (for example if the cloud availability is full) tear down in that cloud.

  <span style="color:#228B22">**Takeaways:**</span>

  1. Vendor-agnostic infrastructure-as-code
  2. Ansible used to provision **`and`** post-provision across clouds
  3. All infra is exposed as yml variable so it's human-friendly to use while still being flexible and powerful
  4. Can leverage the input and ouput of Tower. E.g. we kick it off from hosted services catalog to trigger and post to slack after it's finished but could also be kicked off from any CMDB and integrated with other Chatops.

  <span style="color:#a50000">**Video Demonstration:**</span>

  [![DEMO](http://img.youtube.com/vi/4C5ILW9JRho/0.jpg)](http://www.youtube.com/watch?v=4C5ILW9JRho "Multi-Cloud Workflow"){:target="_blank"}

</details>
</div>
{::options parse_block_html="false" /}