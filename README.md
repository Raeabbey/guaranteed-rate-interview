# CloudFormation Template: Free-Tier VM Setup

This CloudFormation template helps you create a free-tier virtual machine (VM) with the specified objectives using your chosen Infrastructure-as-Code (IaC) tool.

## Objectives

The CloudFormation template aims to achieve the following objectives:

- Create a VM using a 1 GB attached block storage volume with a valid partition table and file system.
- Configure automatic mounting of the filesystem upon reboot of the VM.
- Serve web pages using an appropriate service (e.g., Apache, Nginx, or IIS) that starts automatically upon boot.
- Serve an "index.html" file containing the text "Hello GR World" from the Document Root directory of the attached volume.
- Apply security group rules to restrict traffic to HTTP and either RDP or SSH.
- Associate the VM with a static IP address.


## Additional Notes

- Remember to follow the cloud provider's best practices for managing and securing your resources.
- The CloudFormation template can be further customized or extended to meet your specific requirements.
- Make sure to clean up and delete the stack or resources to avoid incurring any unintended costs.

