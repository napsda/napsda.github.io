# Post-Provisioning Demo
The Post-Provisioning demo (workflow) consists of:
1. Provision a "clean-slate" VM
1. (refresh inventory)
1. Install relevant software
1. Communicate that this has been done

In the case of this example we provision a VM in AWS, post-provision with the [beats lightweight shippers](https://www.elastic.co/beats/), and post to Slack the IP address of the VM.

## Takeaways
1. Unified language used throughout (ansible)
1. Straight-forwardness (simplicity) of each individual process
1. Ease of modification while still maintaining flexibility
1. Ease of integration with additional tools or processes.


## Demo
Check out the video demonstration:

  [![DEMO](http://img.youtube.com/vi/w6hx4Ph0wJw/0.jpg)](http://www.youtube.com/watch?v=w6hx4Ph0wJw "Elk Post Provisioning"){:target="_blank"}