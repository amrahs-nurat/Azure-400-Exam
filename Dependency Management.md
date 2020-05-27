#### Assessment questions for Dependency Management on Microsoft Azure for DevOps Engineers: 

1. You are trying to update a Maven dependency with a same version number in Azure Artifacts, but you get a 409 status code. What would you do to handle this?

- Change the version of the dependency and keep all pom.xml files for all dependent projects with the older version.
- Delete the entire Maven dependency and redeploy it again with same version number.
- Change the version of the dependency and update all pom.xml files for all dependent projects.  ( Correct )
- After updating the dependency, redeploy all projects again.

2. What is the default view when a package feed is created?

- @local  ( Correct )
- @dev
- @prerelease
- @release

3. You created open source software licensed under the terms of the Common Development and Distribution License. Your goal was to integrate this software into the Linux kernel, but your license does not allow this. Why is that?

- Because the source code of Linux is distributed under the terms of the General Public License which does not allow this ( Correct )
- Because the source code of Linux is distributed under the terms of the Apache 2 License which does not allow this
- Because the source code of Linux is distributed under the terms of the MIT License which does not allow this
- Because the source code of Linux is distributed under the terms of the BSD License which does not allow this

4. What is the file type of a NuGet task configuration file?

- .nuspec ( Correct )
- .nuget
- .yml
- .xml

5. What is the default permission for the Project Collection Build Service?

- Reader
- Owner
- Contributor ( Correct )
- Collaborator

6. What would happen after an upstream feed outage lasts less than 12 hours?

- Feeds would work normally because of the metadata cache.  ( Correct )
- All upstreams of the affected package type will automatically be restarted.
- Admins receive an alert notification to redeploy the feeds.
- All upstreams of the affected package type will automatically be deleted.

7. What is one benefit of a personal access token?

- It authenticates other services with Azure DevOps Services  ( Correct )
- It validates a pipeline's access to a production environment
- It enables communication between Azure DevOps Services
- It authenticates APIs with Azure DevOps pipelines

8. You are implementing package management on your solutions and you have large binary packages that you need to manage. What would you do to avoid size limitation issues?

- Partition the binaries into smaller sizes to avoid size limitations.
- Use any package type and configure the package manager to have an unlimited size.
- Use the NuGet package type that is tested for up to 1 TB of size.
- Use the Universal Package type that is tested for up to 1 TB of size.  ( Correct )

9. In which environment does Azure Artifacts comes pre-installed?

- Azure DevOps Server 2018 and 2019
- TFS 2016, 2017, 2018, and 2019
- Azure DevOps Server 2019   ( Correct )
- TFS 2016, 2017, and 2018

10. How many free Azure Artifacts licenses are given to each organization?

- Five  ( Correct )
- Zero
- Three
- Two

11. Components Y and Z both depend on a shared component X, and E depends on Y and Z. what would happen to component E if X releases a new version with breaking changes?

- If X updates, but Y does not, E cannot take A's updates without introducing a dependency endless cycle.
- If Y updates, but Z does not, E cannot take Y's updates without introducing a dependency conflict.  ( Correct )
- If Y and Z update, E cannot take Y's updates without introducing a dependency conflict.
- If X and Y update, E would take the update and run successfully.

12. What does determinism in upstream sources refer to?

- Your feed resolves package requests in order.  ( Correct )
- Your feed resolves package requests randomly.
- Your feed resolves package requests according to priority.
- Your feed resolves package requests starting from the last.

13. What is used to bring packages together from multiple feeds?

- Downstream sources
- Package manager
- Feed explorer
- Upstream sources   ( Correct )

14. What is one of the developed generations of build artifacts?

- Pipeline artifacts   ( Correct )
- Build packages
- DevOps artifacts
- Build artifacts V2

15. What do you need to set to be able to publish an Azure Artifacts feed?

- Project Collection Build Service identity as a Collaborator on the feed
- Project Collection Build Service identity as a Contributor on the feed   ( Correct )
- Project Feed Service identity as a Contributor on the feed
- Project Feed Service identity as a Collaborator on the feed

16. You have a team working on large number of published packages and are using views to promote packages. You need to make sure you track package version releases as soon as they are deployed. What is the best way to handle this?

- Submit a follow action to get notifications whenever a package is promoted.    ( Correct )
- Make sure that every package has a readme file associated to track updates to each package.
- Create an alert to get notified whenever any change is applied.
- Save the view logs and check them frequently to monitor and filter updates.

17. What is used to install Maven artifacts in an Azure DevOps service build?

- Npm
- NuGet
- Spring
- Gradle   ( Correct )

18. You have multiple package feeds for different projects while each project is referencing only one feed. What would you do to use packages from this feed with best practices?

- Use upstream sources to bring multiple projects into a single project.
- Use upstream sources to bring packages from multiple feeds into a single feed.
- Reference only one feed across all projects and ensure you have enough permissions over the feed.
- Ensure you use the same Packages type across all feeds and configure an integrated project containing all projects sources.

19. How can you publish a package to an external NuGet feed?
```
Incorrect -
- task: NuGetCommand
  inputs:
    command: push
    external: true                      
   publishFeedCredentials: '<Name of the NuGet service connection>'
    versioningScheme: byEnvVar
    versionEnvVar: <VersionVariableName>
Incorrect -
- task: FeedCommand
  inputs:
    command: publish
    FeedType: NuGet
   publishFeedCredentials: '<Name of the NuGet service connection>'
    versioningScheme: byEnvVar
    versionEnvVar: <VersionVariableName>"
Incorrect -
- task: FeedCommand@2
  inputs:
    command: push
    FeedType: NuGet    
   publishFeedCredentials: '<Name of the NuGet service connection>'
    versioningScheme: byEnvVar
    versionEnvVar: <VersionVariableName>"
Correct -
- task: NuGetCommand@2
  inputs:
    command: push
    nuGetFeedType: external
    publishFeedCredentials: '<Name of the NuGet service connection>'
    versioningScheme: byEnvVar
    versionEnvVar: <VersionVariableName>
```





