# F5 Configuration
The demo consist of a f5 device configuration being automated by Ansible Automation Platform using two different methods via a Tower survey.

The F5 demo consist of:
1. F5 device configuration by Ansible Automation Platform using two different methods via a Tower survey.
2. F5 BIGIP modules for configuration of Virtual Servers
3. F5 AS3 Templates for Virtual Server configuration

## Takeaways:
1. Unified language used throughout - ansible
1. Ansible Tower survey is used for easy configuration method selection at runtime by using extra-variables. 
1. Variables are collected using `bigip_device_info` module and passed to Slack via API for notification of virtual server configuration

## Demo
Check out the video demonstration:

  [![DEMO](http://img.youtube.com/vi/FGFuXhKPs-s/0.jpg)](http://www.youtube.com/watch?v=FGFuXhKPs-s "F5 configuration with Ansible"){:target="_blank"}
