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

## Instructions

1. **Pre-requisites**: Ensure you have an account with the cloud provider (AWS or Azure) and the necessary IAM/credentials configured for your chosen IaC tool.

2. **Clone the Repository**: Clone or download the repository containing the CloudFormation template and supporting files.

3. **Edit the Template**: Open the CloudFormation template file (e.g., `template.yaml`) and modify any parameters or settings as required. Provide the necessary information for your cloud provider and adjust resource configurations if needed.

4. **Deploy the Stack**: Use your IaC tool's command or interface to deploy the CloudFormation stack. Make sure to provide any required parameters or inputs, such as the stack name and region.

5. **Wait for Deployment**: Monitor the deployment process and wait until the stack creation is complete.

6. **Access the Web Page**: Once the stack is successfully deployed, you can access the web page by entering the VM's static IP address in your web browser. You should see the "Hello GR World" text displayed.

7. **Accessing the VM**: For accessing the VM, follow the appropriate methods based on the cloud provider and your configuration. For example, you may use SSH or RDP to connect to the VM.

## Additional Notes

- Remember to follow the cloud provider's best practices for managing and securing your resources.
- The CloudFormation template can be further customized or extended to meet your specific requirements.
- Make sure to clean up and delete the stack or resources to avoid incurring any unintended costs.

