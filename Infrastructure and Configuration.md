1. When using Azure PowerShell, what is required to deploy a private template into a storage account?

- A SAS token   ( Correct )
- An Oauth Token
- A PAT token
- A JWT Token

2. What type of automation are resource manager templates?

- Declarative    ( Correct )
- Imperative
- Cloud infrastructure
- Managing

3. What are the two types of states in an Azure Security alert?

- Ongoing and Dismissed
- Active and Dismissed     ( Correct )
- Ongoing and Ousted
- Active and Ousted

4. What is required to provide connectivity to a Virtual Machine?

- A Virtual Connection
- A Storage Resource
- A Virtual Network   ( Correct )
- A Resource Group

5. What property can you use to prevent repeated procedures throughout a template?

- Use BSON notation to list the procedures under 'variables'
- Use JSON notation to list the procedures under 'variables'
- Use JSON notation to list the procedures under 'functions'  ( Correct )
- Use BSON notation to list the procedures under 'functions'

6. For a successful Azure Resource Manager (ARM) template for Azure Kubernetes Service (AKS) you must make sure your IP ranges do not clash with public IPs. How would you prevent any clashing?

- Check for the Azure Virtual Network (VNET) IP address’ compatibility with RFC 19.   ( Correct )
- Reduce the IPs in your template to less than 10.
- Increase or decrease the number of pods depending on queue of nodes.
- Monitor the number of nodes to auto-set the number of pods.

7. What deployment mode is used for a nested resource template?

- Incremental mode    ( Correct )
- Incomplete mode
- Parameter mode
- Complete mode

8. You are configuring a Linux Virtual Machine using Ansible in Azure. You are in the process of creating a network security group and would like to allow SSH traffic on TCP port 22. What rule script could you run in your Ansible playbook to accomplish this?

- rules: - name: SSH protocol: Tcp destination_port_range: 22 access: Allow priority: 1001 direction: Inbound     ( Correct )
- rules: - name: SSH protocol: Tcp destination_port_range: 22 access: Deny priority: 101 direction: TrafficInbound
- rules: - name: SSH protocol: Tcp destination_port_range: 22 access: Allow priority: 101 direction: Outbound
- rules: - name: SSH protocol: Tcp destination_port_range: 22 access: Allow priority: 1001 direction: Outbound

9. After successfully creating a nested template, you want to use the 'reference' function in the outputs section of your nested template. What should you do in order to properly use the 'reference' function?

- Convert your nested template to a linked template to return the values for an undeployed resource.
- Convert your nested template to a classic template to return the values for a deployed resource.
- Convert your nested template to a classic template to return the values for an undeployed resource.
- Convert your nested template to a linked template to return the values for a deployed resource.    ( Correct )

10. How would you nest a template within the main template?

- Use the 'mode' property to specify the template syntax.
- Use the 'variablesLink' property to match the version in the nested template.
- Use the 'parametersLink' property to match the version in the nested template.
- Use the 'template' property to specify the template syntax.      ( Correct )

11. You created a release to test the latest changes in your application and the build pipeline was tied to Azure Policy. While the release was in progress to perform an action, the deployment was marked as FAILED. What is the best explanation for this error message?

- The release deployment had an action that was disallowed by the defined policy.   ( Correct )
- A name was not set for the release job.
- There was a missing step to deploy the release to Azure App Services.
- There was a conflicting version of the release.

12. You successfully used Azure Resource Manager (ARM) templates to deploy an Azure Kubernetes Service (AKS) cluster. You set the type on this cluster to VirtualMachineScaleSets. In what scenario would this property be useful?

- You want to increase or decrease the number of nodes depending on demand.  ( Correct )
- You want to monitor a metric to set the number of nodes.
- You want to increase or decrease the number of pods depending on queue of nodes.
- You want to monitor the number of nodes to auto-set the number of pods.

13. You are tasked with making multiple deployments against a particular resource group in Azure CLI. However, when you attempt to make the deployments you receive the "DeploymentQuotaExceeded" error code. What can you do within the CLI to fix this issue?

- Delete entries from your history that are no longer needed with the az group deployment delete command.    ( Correct )
- Delete entries from your history that are no longer needed with the Remove-AzResourceGroupDeployment command.
- Implement new empty entries in your history with the New-AzureRmResourceGroupDeployment command.
- Implement new empty entries in your history with the az group deployment create command.

14. An Azure policy has default built-in policies. Which naming pattern ensures that resource names match the naming convention?

- Require like pattern
- Require tag like pattern
- Allow multiple name pattern
- Require match pattern    ( Correct )

15. You want to deploy an Azure Kubernetes Service (AKS) cluster with advanced networking using an Azure Resource Manager (ARM) template. What is required to deploy advanced networking?

- Apply the "IP Range" to a value that is within an Azure Virtual Network.
- Open GitHub and apply the Credentials and Crucial parameters.
- Apply all default JSON parameters.
- Create a service principal (SP) and use the SP's Application ID, Object ID, and Secret parameters.   ( Correct )

16. You are using Azure PowerShell with Azure Storage to create and manage your resources from the command line. You create a storage account and name it "MainStorage," but Azure is not allowing you to use this name. What is the most likely reason for this issue?

- The name must contain a period (.)
- The name must be all uppercase.
- The name must be all lowercase.      ( Correct )
- The name must contain a hyphen (-).

17. You are assigning a public IP address to a virtual machine using an ARM template. You name the "domainNameLabel" property for your public IP address "MainDomain." Why is Azure not allowing you to use this name?

- The name must contain a hyphen (-).
- The name must be all lowercase.      ( Correct )
- The name must contain a period (.)
- The name must be all uppercase.

18. You are going through the process of creating multiple Virtual Machines and Virtual Networks using an Azure Resource Manager Template. After you finish creating the Virtual Machines you decide to resize one of your VM's disks but receive a "Conflict" error. What is the most likely explanation of this error?

- Disk resizing is only allowed when creating a Virtual Machine, or the Virtual Machine is deallocated.     ( Correct )
- A Virtual Machine within the group already has this size therefore the operation cannot be completed.
- Disk resizing is not allowed in the region or cluster that your VM is located in.
- Disk is unsuccessful because the cluster or region doesn't have resources available, you will have to wait for resources to clear up on the shared resource pool.










