#### Assessment Questions on Continuous Delivery on Azure for DevOps Engineer
#### Note: '( Correct )' is represent to collect answer

1. How can you prepare tasks to be added to a task group?

- Push the tasks to NuGet.
- Update the Git repository for the project as a task group.
- Update all parameters to be defined as variables.    ( Correct )
- Move all tasks to a different Azure account.

2. What best describes a "Gate?"

- A convenient way to get data into various parts of your build pipeline
- Something that grants provision access to user groups
- Something that allows automatic collection of health signals from external services     ( Correct )
- A deprecated variable that modifies how the build agent cleans

3. What Azure DevOps feature can be used to group a set of related deployment activities?

- Task Groups    ( Correct )
- Stages
- Release Gates
- Deployment Groups

4. What Azure DevOps feature allows the release pipeline to get feedback from external system?

- Azure Functions
- Azure DevOps Marketplace
- External Approvers
- Release Gates    ( Correct )

5. For what would you use gates?

- Running with cross-platform scripts
- Tasking a server job
- Incident and issue management     ( Correct )
- Custom stage templates

6. You have an Azure pipeline that requires manual steps for deployments. You want to update your pipeline so that it will release artifacts automatically without any manual intervention. How can you accomplish this?

- Use a predefined schedule or trigger deployments automatically for each pull requests or code commit.   ( Correct )
- Create a test harness that will deploy to production automatically after regression tests succeed in the test environment.
- Use the "continuous release" feature in the Azure pipeline.
- Create a serverless function in Azure that will automatically trigger your pipeline.

7. How can you deploy to a different set of environments in the same Azure DevOps pipeline?

- Use Task Groups
- Use Deployment Groups
- Use Pipeline Stages      ( Correct )
- Use Release Gates

8. What advantage does the security team gain from continuous security validation?

- They can approve the CI/CD process as a whole so they do not have to approve every single release.      ( Correct )
- They can have enough oversight to approve all releases before they are deployed.
- They gain the ability to be apart of each code review, allowing for more control over releases.
- They can configure their own firewall rules to allow internal applications to reach external systems.

9. What do you use to implement blue-green deployment for an application running on Azure VMs?

- Application Insights
- Release Gates
- Internal Load Balancer
- Traffic Manager      ( Correct )

10. You are tasked with making some changes to an application that your team developed. You make the appropriate code changes on your branch of the repo. What two security measures should be used to ensure your application is added to the repository properly?

- Each commit should be linked to a work item and the continuous integration build process should be successful at least once.   ( Correct )
- Each code change should be annotated and commented and the continuous development release process should be successful at least once.
- Each commit should be signed off on by another team member and a code review with the entire team should take place.
- All changes should be put through a unit test and the release pipeline should have a job added to ensure a code review takes place.

11. How can you deploy to three environments at the same time using Azure DevOps Pipeline stage?

- Choose After release as the trigger.   ( Correct )
- Choose Manual as the trigger.
- Choose Automatic as the trigger.
- Choose After stage as the trigger.

12. Which task can be used to ask for a decision from a user?
 
- Manual Intervention    ( Correct )
- Approval
- Invoke REST API
- Delay

13. What term is used to define different steps in the release pipeline?

- Stages     ( Correct )
- Jobs
- Tasks
- Variables

14. Your build pipeline executes a PowerShell script on a VS2017 agent that returns the version of PowerShell the machine is running whether or not WINRM is enabled. What is required in order to make sure this PowerShell script will still be successful after a code change or it is deployed to a different stage?

- Enable continuous deployment on the build pipeline and ensure the script can execute on multiple domains so it can be deployed to other stages.
- Ensure continuous integration is enabled on the build pipeline and publish the script itself as an artifact so it can be used in other stages.   ( Correct )
- Enable unit testing for all code changes and ensure the script can use invoke statements so it can run on a local machine and reach out to other stages.
- Ensure continuous deployment is enabled on the release pipeline and return the PowerShell version from the script to be certain in can be used in other stages.

15. What is the easiest way to add a test environment?

- Save the release definition and queue a new release.
- Have an artifact promotion strategy.
- Use cloud infrastructure to create environments dynamically.
- Use the clone environment option.    ( Correct )

16. What is the scope of a task group?

- A task group can only be used in the same pipeline.
- A task group can only be used on the same machine as the application.
- A task group can only be used within build pipelines.
- A task group can only be used on the project level.    ( Correct )

17. What aspect of code do automated tests within the CI process measure?

- Integrity
- Length
- Functionality
- Quality     ( Correct )

18. What is true about the blue-green deployment pattern with Azure DevOps?

- It can only be used with cloud applications.
- It is used to speed up the release process.
- It uses a mirror production environment with the latest release and exposes it only to a subset of users.     ( Correct )
- It updates a subset of production servers with the latest release and gradually move to the remaining servers.




