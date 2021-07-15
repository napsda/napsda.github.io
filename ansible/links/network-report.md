# Dynamic Documentation

The demo consist of a network device report hosted in a long-running web server. A daily scheduled job in Ansible Tower updates the report.

## Takeawys

1. Ansible is used as a unifying language across vendors. Ansible logs into every device.
1. Variables are collected using `gather facts`, essentially using Ansible's built-in library.
1. Variables are rendered using the powerful [Jinja2](https://jinja.palletsprojects.com/en/2.11.x/) templating library.


## Demo
Check out the video demonstration:

  [![DEMO](http://img.youtube.com/vi/AOhIiDYiel8/0.jpg)](http://www.youtube.com/watch?v=AOhIiDYiel8 "Network Reporting"){:target="_blank"}

## Repository
  [network](https://gitlab.com/redhatautomation/network){:target="_blank"}  
