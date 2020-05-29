#### Assessment Questions for Code Flows on Microsoft Azure for DevOps Engineer
#### Note: '( Correct )' is using to refer the Correct answer.

1. What Bitbucket supported Azure pipe allows you to run commands using the Azure CLI?

- Azure CLI Configure
- Azure ARM Deploy
- Azure CLI Run      ( Correct )
- Azure ARM Configure

2. You are using Azure Storage with a Jenkins continuous integration solution and want to automate uploading your build artifacts to your storage account. You decide to use a pre-build action but the files are not uploading. What should you do?

- Incorrect -Change from a pre-build action to a webhook.
- correct -Change from a pre-build action to a post-build action.
- Incorrect -Change from a pre-build action to a copy artifact.
- Incorrect -Change from a pre-build action to a storage artifact.

3. You are trying to adopt a successful Git branching strategy. You have a master branch and a release branch and are trying to port changes made in your release branch into your master. How would you commit specific changes into your master branch?

- Incorrect -git commit <commit-hash>
- incorrect -git merge <commit-hash>
- Incorrect -git rebase <commit-hash>
- Correct -git cherry-pick <commit-hash>

4. You have been using the builder pattern to build your docker images. Doing this has caused you to maintain multiple files for development and production builds. What can you do to only maintain one Dockerfile for all your environments?

- Incorrect -Use multiple COPY statements in your Dockerfile.
- Incorrect -Use multiple WORKDIR statements in the Dockerfile.
- Correct -Use multiple FROM statements in the Dockerfile.
- Incorrect -Use multiple RUN statements in the Dockerfile.

5. Azure allows integration with BitBucket and GitHub, what is one difference between GitHub and Bitbucket?

- Incorrect -Bitbucket only hosts projects that use the Git VCS while GitHub also supports the Mercurial VCS in addition to Git.
- Correct -GitHub only hosts projects that use the Git VCS while Bitbucket also supports the Mercurial VCS.
- Incorrect -GitHub is a version control system that uses components of Git while Bitbucket is a web-based version control repository.
- Incorrect -Bitbucket is a version control system that uses components of Git while GitHub is a web-based version control repository.

6. Your organization has been using open source software as part of product development, but you recently found out that some of the software has vulnerabilities. What approach can you take to ensure that you can catch this early on in your CI/CD pipeline?

- Incorrect -As part of your CI/CD pipeline, implement Jenkins OSS to see reports of all third-party packages in your solution.
- Incorrect -As part of your CI/CD pipeline, implement Azure vNext to see reports of all third-party packages in your solution.
- Incorrect -As part of your CI/CD pipeline, implement Active Scan to see reports of all third-party packages in your solution.
- Correct -As part of your CI/CD pipeline, implement WhiteSource Bolt to see reports of all third-party packages in your solution.

7. Your team is using TFVC in Azure DevOps. They used the 'destroy' command to delete a feature branch that was no longer necessary. You need to access this branch a few weeks later so you go through the deleted items section in the Source Control Explorer, but cannot locate your branch anywhere. What is the explanation for this issue?

- Incorrect -TFVC permanently deletes any deleted feature branches after one week.
- Correct -The destroy command causes a permanent delete.
- Incorrect -The destroyed items section in Source Control explorer should have been checked instead of the deleted items section.
- Incorrect -The destroy command causes deleted files to be stored in Solution Explorer instead of Source Control explorer.

8. You are using Git for your Azure Devops project and set up a policy that blocks others from pushing to your master branch. You are the administrator of your project and have also blocked yourself. What can you do to ignore this policy without replacing it?

- Correct -Give yourself the "Bypass policies when pushing" permission.
- Incorrect -Pass in the -f to the git push command.
- Incorrect -Give yourself the "Ignore policies when completing pull requests" permission.
- Incorrect -Add your user id to the .gitignore file.

9. Your organization implemented rigid processes for open source software to reduce the potential of data breaches. You have to continuously check these packages for vulnerabilities. What tool can you use to accomplish this as part of your DevOps process?

- Incorrect -Azure Scan
- Incorrect -Contoso
- Correct -WhiteSource Bolt
- Incorrect -RedHat Source

10. What is the definition of trunk-based development?

- Correct -A source-control branching model where developers collaborate on code in a single branch.
- Incorrect -A configuration management development model where developers collaborate on code in multiple branches.
- Incorrect -A configuration management development model where developers collaborate on in a single branch.
- Incorrect -A source-control branching model where developers collaborate on code in multiple branches.

11. What is the difference between default pull request templates and branch-specific pull request templates?

- Correct -Default templates are automatically applied for all new pull requests in the repository, while branch-specific templates are automatically applied to pull requests targeting a specific branch.
- Incorrect -Default templates have to be manually applied for all new pull requests in the repository, while branch-specific templates are automatically applied to pull requests targeting a specific branch.
- Incorrect -Default templates are automatically applied to pull requests targeting a specific branch, while branch-specific templates are automatically applied for all new pull requests in the repository.
- Incorrect -Default templates are automatically applied for all new pull requests in the repository, while branch-specific templates have to be manually applied to pull requests targeting a specific branch.

12. You want to configure your Git repository to use a different default branch to merge code into when your team creates new pull requests. What must you do to accomplish this?

- Incorrect -Edit Security permissions on your Git repository.
- Correct -Edit Policies permissions on your Git repository.
- Incorrect -Cherry-pick your default branch with your second branch.
- Incorrect -Merge your default branch with your second branch.

13. What is the purpose of using a consistent naming convention on your feature branches in Git?

- Correct -It allows you to identify the work done in a branch
- Incorrect -It allows you to prevent merge conflicts
- Incorrect -It allows you to identify the work done in your release feature toggles
- Incorrect -It allows you to prevent bypassing branch policies

14. You integrated TFVC into Azure Devops and are using the main-only branching strategy. What should you do after completing a release cycle to stabilize the release and continue development for your next version in main?

- Incorrect -Create a release build.
- Correct -Create a release branch.
- Incorrect -Create a feature build.
- Incorrect -Create a feature branch.

15. When using Azure Pipelines, pull request triggers are capable of what significant function?

- Incorrect -Creating a feature every time a new version of the selected artifact is available as part of a pull request.
- Correct -Creating a release every time a new version of the selected artifact is available as part of a pull request.
- Incorrect -Creating a pull request every time a new version of the selected artifact is available as part of a pull request.
- Incorrect -Creating a default pull request template every time a new version of the selected artifact is available as part of a pull request.

16. What technique allows teams to modify system behavior without changing code?

- Incorrect -Forward integration
- Incorrect -Pull requests
- Correct -Feature flagging
- Incorrect -Reverse integration

17. You manage a small team of software developers who are all working on a project using Azure Repos. You want to make sure that everyone reviews their changes before completing a pull request. What can you do to enforce this rule?

- Incorrect -Give your team members the "Pull requests review required" permission.
- Incorrect -Enable "Pull requests review required" under branch policies and set the number of reviews you want to require.
- Correct -Enable "Require a minimum number of reviewers" under branch policies and set the number of reviews you want to require.
- Incorrect -Give your team members the "Require a minimum number of reviewers" permission.

18. You recently encountered multiple merge conflicts while using Git in your Azure Repos repository. You were able to clean up your file and solve all your conflicts. What final steps must you complete to completely wrap up?

- Correct -Mark each conflicted file as solved using the git add <filepath> command and commit the resolution with the git commit command.
- Incorrect -Mark each conflicted file as solved using the git resolve <filepath> command and commit the resolution with the git commit command.
- Incorrect -Mark each conflicted file as solved using the git add <filepath> command and commit the resolution with the git config command.
- Incorrect -Mark each conflicted file as solved using the git init <filepath> command and commit the resolution with the git commit command.

------------------------------------

1. You led a small development project that is now completed. You need to provide a record of the development operations tied with your team's pull requests, but are struggling to trace back each specific instance. What would you do to prevent this work?

- Incorrect -Set the "Enforce a merge strategy" policy.
- Incorrect -Set the "Build validation" policy.
- Incorrect -Set the "Check for comment resolution" policy.
- Correct -Set the "Check for linked work items" policy.

2. You want to install a Virtual Machine Agent but you forgot the administrator password for your Windows Virtual Machine. What action can you take to install the VM Agent?

- Incorrect -Install it in express mode.
- Correct -Install it in offline mode.
- Incorrect -Install it in online mode.
- Incorrect -Install it in general mode.

3. How would you classify Checkmarx, BinSkim, and WhiteSource?

- Incorrect -Tools that run dynamic code analysis tests to ensure that your code is following all rules for maintenance and security
- Correct -Tools that run static code analysis tests to ensure that your code is following all rules for maintenance and security
- Incorrect -Tools that allow you to collaborate with other engineers and designers on your team
- Incorrect -Tools that allow you to continuously integrate your code with every commit

4. What is the function of Git LFS?

- Incorrect -Handling frequently updated small projects by providing the ability to track changes
- Incorrect -Reducing the impact of frequently updated small files in your repository
- Correct -Reducing the impact of large files in your repository
- Incorrect -Handling large projects by providing the ability to track changes

5. How would you configure your registry authentication to have role-based access control?

- Incorrect -Using container principals
- Incorrect -Using JWT tokens
- Correct -Using service principals
- Incorrect -Using a bearer token

6. Your project is held in an Azure Repos repository. Recently, a bug was introduced after a long series of commits. What can you do to make this search process more efficient How would you most efficiently track down and locate this bug?

- Incorrect -git init good or git init bad
- Correct -git bisect good or git bisect bad
- Incorrect -git config good or git config bad
- Incorrect -git debug <revision>

7. What step must a client application complete when requesting an access token?

- Incorrect -Defining the permissions that can be granted to other pipelines
- Incorrect -Defining the permissions that can be granted to other applications
- Incorrect -Specifying the desired HTTP verbs in the scope parameter of the request
- Correct -Specifying the desired permissions in the scope parameter of the request

8. What is the difference between Development Isolation and Feature Isolation?

- Incorrect -Feature Isolation allows you to branch one or more release branches from main, whereas Development Isolation branches uses development branches.
- Correct -Feature Isolation allows you to branch one or more feature branches from main, whereas Development Isolation uses develop branches.
- Incorrect -Development Isolation allows you to branch one or more feature branches from main, whereas Feature Isolation uses development branches.
- Incorrect -Feature Isolation allows you to branch one or more release branches from main, whereas Development Isolation uses feature branches.

9. Which TFVC strategy allows for concurrent release management, multiple and parallel releases, and codebase snapshots at release time?

- Incorrect -Main Only
- Incorrect -Feature Isolation
- Incorrect -Development Isolation
- Correct -Release Isolation
