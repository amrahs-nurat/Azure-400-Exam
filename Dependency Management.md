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
-----------------------------------------------------------
1. What is an example of a technique used by advanced Software Composition Analysis tools on open source components?

- Incorrect -Running dynamic code analysis tests to ensure that your code is following all rules for both maintenance and security
- Incorrect -Running dynamic code analysis tests that execute penetration tests on your local machine
- Incorrect -Cross referencing every function and variable in your code with your organizational policies
- Correct -Cross-referencing every open source component found in your code with your organizational policies and failing a build when violation happens

2. When designing and deploying software, how would you classify CVE, CWE, and CVSS?

- Incorrect -Systems that improve software development speed in complex environments
- Correct -Measurement and risk mitigation efforts focused on realizing software assurance
- Incorrect -Management and tracking efforts focused on realizing network monitoring
- Incorrect -Systems that allow for continuous integration of code

3. You deployed an open source component into your development environment and would like to ensure it aligns with your company policies. After implementing Software Composition Analysis tools, you want to run more measures to meet security requirements. What can you implement to accomplish this?

- Incorrect -Integration testing
- Correct -Static code analysis
- Incorrect -Dynamic code analysis
- Incorrect -Integration analysis

4. How would you avoid duplicates when automatically pushing NuGet packages in each release?

- Incorrect -Perform an automatic delete to all packages before the new release is deployed.
- Incorrect -On NuGet Push, remove duplicates.
- Correct -On NuGet Push, allow duplicates to be skipped.
- Incorrect -After deployment, manually review and remove duplicates.

. How would your NuGet package sources be configured for your feed to provide deterministic restore?
```
Incorrect -
"<pSources>
  <add name=""FabrikamFiber"" value=""https://pkgs.dev.azure.com/fabrikam/_packaging/FabrikamFiber/nuget/v3/index.json"" />
</pSources>"

Incorrect -
<packageSources>
  <add key="FabrikamFiber" name="https://pkgs.dev.azure.com/fabrikam/_packaging/FabrikamFiber/nuget/v3/index.json" />
</packageSources>

Incorrect -
<pSources>
  <clear />
  <add name="FabrikamFiber" value="https://pkgs.dev.azure.com/fabrikam/_packaging/FabrikamFiber/nuget/v3/index.json" />
</pSources>

Correct -
<packageSources>
  <clear />
  <add key="FabrikamFiber" value="https://pkgs.dev.azure.com/fabrikam/_packaging/FabrikamFiber/nuget/v3/index.json" />
</packageSources>
```
6. How would you configure publishing for NPM packages to Azure Artifacts feed?
```
Incorrect -
- task: Npm
  inputs:
    command: publish
    publishRegistry: useNpmFeed
    publishFeed: feedName

Correct -
- task: Npm@1
  inputs:
    command: publish
    publishRegistry: useFeed
    publishFeed: feedName

Incorrect -
- task: Npm@1
  inputs:
    command: deploy
    publishRegistry: useArtifactsFeed
    publishFeed: feedName

Incorrect -
- task: Npm
  inputs:
    command: deploy
    publishRegistry: useNpmFeed
    publishFeed: feedName
```

7. What would you do to make sure data is maintained within packages?

- Correct -Use package repositories to maintain a database of the key application metadata containing name, description, maintainer, dependencies and version information.
- Incorrect -Use a relational database to maintain data through each deployed package settings file which is saved in version control.
- Incorrect -User version control to maintain a database of the key package files containing configuration, description, settings and version information.
- Incorrect -Use local storage to maintain a data log for each package version saved in the release storage containing name, description, dependencies and version information.

8. You work for a private mobile application development company and need to find an open source software license for a new application. After implementing a Copyleft license, you are accused of violating company policy and negatively affecting the business's competitive advantage. What is the most likely explanation for this?

- Incorrect -Copyleft allows you to do anything you want with code, but requires you to provide attribution to the author.
- Incorrect -Copyleft allows you to incorporate your application into a closed software project that you do not provide the source to.
- Correct -Copyleft would require your company to distribute modified and extended versions of your application to the public.
- Incorrect -Copyleft has frequent vulnerabilities that, if accessed by hackers, could result in private information getting leaked.

9. You have a Maven project and need to generate a Maven artifact on your local machine and assign it to a specific group. What would you do to implement this?
```
Incorrect -
mvn -B archeOp:generate -DarchetypeGroupId="org.apache.npm.archetypes" -DgroupId="MyGroup" -DartifactId="myFirstApp"

Incorrect -
npm -B archeOp:generate -DarchetypeGroupId="org.apache.npm.maven.archetypes" -DgroupId="MyGroup" -DartifactId="myFirstApp"

Incorrect -
npm -B archetype:create -DarchetypeGroupId="org.apache.maven.archetypes" -DgroupId="MyGroup" -DartifactId="myFirstApp"

Correct -
mvn -B archetype:generate -DarchetypeGroupId="org.apache.maven.archetypes" -DgroupId="MyGroup" -DartifactId="myFirstApp"
```

10. What are the possible views for Azure DevOps Services feeds?

- Incorrect -@dev, @prerelease, and @release
- Incorrect -@local, @prerelease, and @production
- Correct -@local, @prerelease, and @release.
- Incorrect -@local, @predeploy, and @deploy

11. What service scans the open source software components identified in an Azure Container Registry image?

- Incorrect -Network Watcher
- Correct -Black Duck
- Incorrect -SoftNAS Cloud
- Incorrect -NetApp

12. What is the concern with sharing components' binaries using source control?

- Incorrect -Binaries can result in inconsistent code between different machines.
- Incorrect -Binaries can result in security risk in your repository.
- Correct -Binaries can significantly increase the size of your repository.
- Incorrect -Versioning is not allowed for binaries in source control.

13. You have packages promoted to the @prerelease view then to the @release view, but you find out these packages are not found by any external teams. What would you do to fix this?

- Incorrect -Make sure that the teams have visual studio professional edition installed.
- Incorrect -Ensure that your @release view and @prerelease view are secure and risk free across the organization.
- Correct -Ensure that your @release view and @prerelease view are visible across the organization.
- Incorrect -Make sure that all external teams have permissions to access the organization's network.

14. Where can you publish NPM packages produced by your build?

- Incorrect -Azure Artifacts, VSTS Package service or Other registries such as https://registry.mavenjs.org/
- Incorrect -Git Package Management service or Azure Artifacts
- Incorrect -Azure Artifacts or other git repos
- Correct -Azure Artifacts, TFS Package Management service or Other registries such as https://registry.npmjs.org/

15. You are creating an open source browser and want to make sure that anyone whomakes changes to it must make them publicly available. What type of license can you implement into your project to accomplish this?

- Incorrect -Attribution, as it allows other to distribute, remix, tweak, and build upon your work
- Correct -Copyleft, as it gives people the right to freely distribute copies and modified versions of your work
- Incorrect -Copyright, as it gives people the right to freely distribute copies and modified versions of your work
- Incorrect -Alteration, as it allows others to distribute, remix, tweak, and build upon your work

16. What is necessary to continue using Azure Artifacts after your trial expires?

- Incorrect -Azure Artifacts trial extension or Visual Studio Professional subscription
- Incorrect -Azure Artifacts license or Visual Studio Professional subscription
- Correct -Azure Artifacts license or Visual Studio Enterprise subscription
- Incorrect -Azure Artifacts trial extension or Visual Studio Community subscription

17. What does the following code do?
- task: NuGetCommand@2
  displayName: 'NuGet push'
  inputs:
    command: push
    publishVstsFeed: '<feedName>'
    allowPackageConflicts: true
  
- Incorrect -It pushes a NuGet package to any type of source control
- Correct -It publishes a NuGet package to an Azure Artifacts feed
- Incorrect -It publishes a NuGet package to an external NuGet feed
- Incorrect -It creates a NuGet package feed

18. What is one main use for build artifacts?

- Correct -To help store build outputs and intermediate files between build steps
- Incorrect -To help store and build integration pipeline and validations steps
- Incorrect -To help store build inputs and settings at the start of each build step
- Incorrect -To help store build inputs and intermediate scripts between release steps

19. You changed your builds to run at project scope but after this change you are receiving access errors to your feed. What would you do to fix this?

- Incorrect -Create a new build identity with default permissions.
- Incorrect -Reset project scope permissions to defaults.
- Incorrect -Add the project-level build identity as an Owner.
- Correct -Add the project-level build identity as a Reader or Contributor.

20. You need to find an open source component that integrates well with your project. A major requirement is to find one that gives you full freedom to use it commercially. What open source software license would meet the requirement?

- Incorrect -Attribution License
- Correct -MIT License
- Incorrect -Attribution-NonCommercial-NoDerivs License
- Incorrect -Public Copyright License

21. You got an instance of TFS disconnected from the internet but you were unable to purchase licenses from the marketplace and have no intention of getting this instance connected. How can you handle this?

- Correct -Assign licenses purchased through an enterprise agreement.
- Incorrect -Make sure all your TFS instances are always connected to the internet.
- Incorrect -Assign licenses purchased through setting up an unlimited license policy.
- Incorrect -Make sure all your TFS instances are always disconnected to the internet.

22. Why should one be wary with licenses in open source software?

- Incorrect -They could contain malware inside that may corrupt your projects.
- Incorrect -They may not integrate well with your code and potentially delete code fragments.
- Correct -They could come with unusual restrictions that may negatively affect your organization.
- Incorrect -They could contain vulnerabilities that will give hackers a gateway to your software.

---------------------------------------------------------------------

1. What is one benefit of a personal access token?

- Correct -It authenticates other services with Azure DevOps Services
- Incorrect -It validates a pipeline's access to a production environment
- Incorrect -It authenticates APIs with Azure DevOps pipelines
- Incorrect -It enables communication between Azure DevOps Services

2. What is the .artifactignore file responsible for?

- Incorrect -It controls what files are uploaded when you publish a NuGet Package.
- Incorrect -It controls package dependencies to ignore when you publish either NuGet package or a Pipeline Artifact.
- Correct -It controls what files are uploaded when you publish either a Universal Package or a Pipeline Artifact.
- Incorrect -It controls package dependencies to ignore when you publish either NuGet or npm package.

3. What is one challenge of package composition?

- Correct -Diamond dependencies
- Incorrect -Multiple team collaboration conflict
- Incorrect -Two-way dependencies
- Incorrect -Infinite conflict

4. How can you publish your packages to an external Universal Packages feed?

- Correct -Create a service connection to point to that feed, then fill in the feed URL and a personal access token to connect them.
- Incorrect -In the .yml file, set Enable external Universal Packages to true, then all packages will be published to that feed automatically.
- Incorrect -Create a personal access token connection to that feed, then publish all the packages directly to the external Universal Packages feed.
- Incorrect -Publish the package to an Azure Artifacts feed, then set the Project Collection Build Service identity to be a Contributor on the feed.

5. In which environment does Azure Artifacts comes pre-installed?

- Incorrect -TFS 2016, 2017, and 2018
- Correct -Azure DevOps Server 2019
- Incorrect -TFS 2016, 2017, 2018, and 2019
- Incorrect -Azure DevOps Server 2018 and 2019

6. What would you do if you were unsure whether you needed more than five Azure Artifact's licenses to your organization?

- Correct -Start a free trial. Every user will be granted access until the end of the trial period, which will revert licenses back to a limit of five.
- Incorrect -Send a request to the support team to apply more free licenses to your organization with a limit of 500 users.
- Incorrect -Start a free trial. Ten users will be granted access until the end of the trial period, which will revert licenses back to a limit of five.
- Incorrect -Purchase more licenses as backup without a limited number of users.

7. You uploaded a package with version 2.0 to Azure DevOps service then realized you need a quick fix, so you upload it again under version 2.0. What is wrong with this approach?

- Incorrect -The immutability constraint won't allow any uploaded packages to be edited or changed even if the package version is new.
- Incorrect -The immutability constraint won't allow uploading a newer revision package with the same version number, as it only allows deleting it and uploading a new package of the same version.
- Correct -The immutability constraint won't allow uploading a newer revision package with the same version number, or delete it and upload a new package of the same version.
- Incorrect -The immutability constraint will require mandatory delete for all previous versions before uploading the updated package.

8. What would you do to prevent sources from overriding well-known packages with altered or incompatible versions?

- Incorrect -Permanently delete all incompatible versions.
- Incorrect -Place any public upstreams last in your resolution order.
- Correct -Place any public upstreams first in your resolution order.
- Incorrect -Delete all incompatible versions from your resolution order.

9. What is true of project team permissions?

- Incorrect -Your project team is assigned to collaborator permission by default.
- Incorrect -Your project team cannot have permissions unless an access policy is created for the package feeds.
- Correct -Your project team is assigned to reader permission by default.
- Incorrect -Your project team has no permissions by default and needs to be set after creation.

