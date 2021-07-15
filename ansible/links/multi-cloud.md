# Multi-Cloud demo

The multi-cloud demo (workflow) consists of:
1. Provision VMs in (1) Azure and (2) AWS
1. In AWS configure an Apache server, in Azure an IIS server.
1. Post in slack channel that multi-cloud workflow has finished.
1. If any of the process fails (for example if the cloud availability is full) tear down in that cloud.

## Takeaways

1. Vendor-agnostic infrastructure-as-code
1. Ansible used to provision *and* post-provision across clouds
1. All infra is exposed as yml variable so it's human-friendly to use while still being flexible and powerful
1. Can leverage the input and ouput of Tower. E.g. we kick it off from hosted services catalog to trigger and post to slack after it's finished but could also be kicked off from any CMDB and integrated with other Chatops.

## Demo
Check out the video demonstration:

  [![DEMO](http://img.youtube.com/vi/4C5ILW9JRho/0.jpg)](http://www.youtube.com/watch?v=4C5ILW9JRho "Multi-Cloud Workflow"){:target="_blank"}

## Repository
https://gitlab.com/redhatautomation/aws
https://gitlab.com/redhatautomation/azure