#### Assessment Questions for Continuous Integration on Microsoft Azure for DevOps Engineers
#### Note: The '( Correct )' Key represent the correct Answer of the question.

1. Your team is deploying a Linux-based application through the build pipeline but does not have an on-prem Linux OS agent to run it. As an administrator of an agent pool, you register a new on-prem Linux OS agent. What are the next steps required to set up the agent to connect with your Azure build pipeline?

- Generate a secret to be used every time the agent connects to the agent pool. Create the secret in the security section of Azure DevOps by giving it a name and a lifespan.
- Generate a LDAP token to be used for the lifespan of the agent. Create the token in the LDAP section of Azure DevOps by giving it a name and a lifespan.
- Generate a personal access token for agent registration in the security section of Azure DevOps by giving it a name and a lifespan  ( Correct )
- Generate a secure key for agent registration in the security section of Azure DevOps by giving it a name and an encryption key.

2. What Azure stack components are required to build a hybrid connectivity deployment?

- An "Azure StackAdmin" must deploy the application service, create a tenant subscription and add a Windows Server 2012 R2 image.
- An "Azure Admin" must deploy the application service, create a tenant subscription and add a Windows Server 2008 image.
- An "Azure Stack Operator" must deploy the application service, create a tenant subscription and add a Windows Server 2016 image.  ( Correct )
- An "Azure Stack Automater" must deploy the application service, create a tenant subscription and add a Windows Server 2012 image.

3. Given policy definition below in the JSON userpolicy.json, what PowerShell commandlet would create a parameterized policy named userPolicy with the definition from the JSON file?
```
[
   {
      "policyDefinitionId": "definitions/policy/464dbb85-3d5f-4a1d-bb09-187a4f81c498",
      "parameters": {
         "tagName": {
            "value": "Department"
         },
         "tagValue": {
            "value": "[parameters('deptValue')]"
         }
      }
   }
]
```

- New-AzPolicySetDefinition -Name 'userPolicy' -PolicyDefinition D:\userpolicy.json -Parameter '{ "deptValue" }'
- New-AzPolicySetDefinition -Name 'userPolicy' -PolicyDefinition D:\userpolicy.json  '{ "deptValue": { "type": "boolean" } }'
- New-AzPolicySetDefinition -Name 'userPolicy' -PolicyDefinition D:\userpolicy.json -Parameter '{ "deptValue": { "type": "string" } }'  ( Correct )
- New-AzPolicySetDefinition -Name 'userPolicy' -PolicyDefinition D:\userpolicy.json -Params '{ "Department": { "type": "string" } }

4. When creating an initiative policy definition, what is the definition location used for?

- The definition location is used to set the drive location of where the policy will be executed.
- The definition location is used to set the job location of where the policy will be published.
- The definition location is used to set the management group or subscription location of where the policy will be stored.  ( Correct )
- The definition location is used to set the executable location of where the policy will be run from.

5. How does a policy definition work?

- It creates a link between the user and a policy group.
- It details the condition in which a policy would be enforced.   ( Correct )
- It defines use cases that are permissible for an application.
- It provides guidance on what a user should or should not do, but does not stop them from performing a task.

6. How should Azure DNS be configured so users can access the Azure Stack instances of your web app?

- For Azure Global access, add the Azure Stack hostname to your web app by creating an CNAME for the web app. Once that is complete, create an A record for the web app and map it to the previously created CNAME for the web application.
- For Azure global access, add the Azure Stack hostname to your web app by creating an MX record for the web app. Once that is complete, create a CNAME for the web app and map it to the previously created MX record for the web application.
- For Azure Stack access, add the Azure Stack hostname to your web app by creating an AA record for the web app. Once that is complete, create a CNAME for the web app and map it to the previously created AA record for the web application.
- For Azure Stack access, add the Azure Stack hostname to your web app by creating an A record for the web app. Once that is complete, create a CNAME for the web app and map it to the previously created A record for the web application.   ( Correct )

7. What PowerShell commandlet would create a VPN gateway that uses a site-to-site connection type?

- New-AzVPNGateway -Name $name -ResourceGroupName $RG -Location $Loc -VPNType RouteBased
- New-AzVirtualNetworkGateway -Name $name -ResourceGroupName $RG -Location $Loc -GateWayType VPN    ( Correct )
- New-AzVirtualNetworkGateway -Name $name -ResourceGroupName $RG -Location $Loc -VPNType VPN
- New-AzVPN -Name $name -ResourceGroupName $RG -Location $Loc -Type VPN

8. You have downloaded Packer and created an windows VM image named win2016 from a template file. What code snippet shows how you would use that image to build a new VM named vmwd123 in Azure using PowerShell?

- New-AzVM -Name "vmwd123" -Image "win2016"    ( Correct )
- New-AzServer -Name "vmwd123" -PackerImage "win2016"
- New-AzVirtualMachine -DisplayName "vmwd123" -Template "win2016"
- New-VMConfig -DisplayName "vmwd123" -Image "win2016"

9. If a task within a task group contains a value for the parameter named "count," why can't the parameter be configured in the pipelines that use the task group?

- The parameter is globally defined.
- The parameter is not defined as a variable so the value cannot be changed.   ( Correct )
- The parameter is not correctly initialized.
- The parameter uses private variables that cannot be changed on the global level.

10. How can you handle regression tests that may take hours to run?

- Enable Test Impact Analysis within the Visual Studio Test task so the only tests run are those relevant to the code committed.  ( Correct )
- Enable Test CI Integration within the Visual Studio Test task so the only tests run are those relevant to the newest code.
- Enable Test Continuous Deployment within the Visual Studio Test task so the tests only apply to code written in the main controller file.
- Enable Test Pipeline Analysis within the Visual Studio Test task so tests are run in parallel.

11. What file format is required for creating Packer templates?

- XML
- YAML
- JSON    ( Correct )
- JS

12. You want a build pipeline script to stop whenever it encounters an error to prevent deployments of faulty artifacts. What YAML file script could be used with PowerShell to output the agent ID of the build and set the script to stop when it encounters an error?

```
Incorrect -
-task: PowerShell@2     
     inputs:                 
            targetType: inline                 
            inline: Write-Host "My ID is $Env:AGENT_ID."                 
            errorActionPreference: exit```
correct -
```-task: PowerShell@2
     inputs:
            targetType: inline
            script: Write-Host "My ID is $Env:AGENT_ID."
            errorActionPreference: stop```
Incorrect -
```-task: Ps@2     
     inputs:                 
            targetType: script                 
            command: Write-Host "My ID is $Env:AGENT_ID."                 
            errorActionPreference: exit```
Incorrect -
```-task: PS@1     
     inputs:                 
            targetType: script                 
            script: Write-Host "My ID is $Env:AGENT_ID."                 
            errorActionPreference: stop
```

13. Which SonarCloud task defines the connection configuration for later tasks?

- Gather Information on SonarCloud
- Prepare analysis on SonarCloud     ( Correct )
- Test Config on SonarCloud
- Create config on SonarCloud

14. What steps are required before naming and categorizing a task group?

- The project must be uploaded to TFS and configured for hybrid deployment.
- All parameters must be linked and the PowerShell Azure module must be imported.
- All parameters must be unlinked and you must select the desired tasks to include.    ( Correct )
- All templates must be saved and their variables unlinked.

15. What code snippet shows a YAML file with a job that runs independently of another job's success or failure?

- jobs:- job: Job1  steps:  - script: echo Job Executed    condition: failed()- job: Job2  dependsOn: Job1  condition: successed()
- jobs:- job: Job1  steps:  - script: echo Job Executed    condition: succeeded()- job: Job2  dependsOn: Job1  condition: always()  ( Correct )
- jobs:- job: Job1  steps:  - script: echo Job Executed    condition: canceled()- job: Job2  dependsOn: Job1  condition: independent()
- jobs:- job: Job1  steps:  - script: echo Job Executed    condition: always()- job: Job2  dependsOn: Job1  condition: failed()

16. What YAML file code snippet runs the Visual Studio Test Task for an environment where you need to run tests from a test plan that has automated test methods?

```
- task: VSTest@1
  inputs:
    testSelector: 'testRun'
    testPlan: tp1
    testConfiguration: tc1
Incorrect -
- task: VSTest@1
  inputs:
    testSelector: 'testRun'
    testPlan: tp1
    testSuite: ts1
Incorrect -
- task: VSTest@2
  inputs:
    testSelector: 'testAssemblies'
    testPlan: tp1
    testSuite: ts1
    testConfiguration: tc1
Your choice: correct -
- task: VSTest@2
  inputs:
    testSelector: 'testPlan'
    testPlan: tp1
    testSuite: ts1
    testConfiguration: tc1
```

17. What level of access is required by default for a user in a DevOps organization to build a pipeline?

- Administrator    ( Correct )
- Read/write
- Read
- Write

18. What Test plan category type can be added to a test plan without being part of a test suite?

- Test case.     ( Correct )
- Test exercise.
- Unit Test.
- Test scenario.



