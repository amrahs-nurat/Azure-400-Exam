#### Assessment Questions for Continuous Feedback on Azure for DevOps Engineer
#### Note: '( Correct )' is used to represent the correct answer.

1. You are asked to export Azure Monitoring data to an external system. How would you accomplish this quickly within Azure Monitor?

- Export the data via a flat CSV file. Format the file in a way that the third party tool can consume the data.
- Create synchronous API between Azure Monitor and the third party tool.
- Create an asynchronous API between Azure Monitor and the third party tool.
- Forward the data through Azure Event Hubs. Afterwards, the third party tool can import the streaming data directly.  ( Correct )

2. Where could an end user provide feedback once they have access to Azure DevOps?

- Under Test Plans
- Under Overview
- Under Repos
- Under Boards     ( Correct )

3. What Analytics Query would you use to find what browsers your users utilize?

```
Correct -
pageViews

| summarize count() by client_Browser

Incorrect -
browser

| join count() by pageViews

Incorrect -
pageViews

| join count() by client_Browser

Incorrect -
browser

| summarize count() by pageViews
```

4. In C#, how would you track an event called "MyEvent"?

- InsightClient myClient = new InsightClient(); myClient.TrackEvent("MyEvent");
- appInsights myClient = new appInsights(); myClient.TrackEvent({name}:"MyEvent");
- appInsights myClient = new appInsights();
  myClient.TrackEvent("MyEvent");
- TelemetryClient myClient = new TelemetryClient(); myClient.TrackEvent("MyEvent");     ( Correct )

5. You'd like to add logging analytics to your Azure Monitor to get a better view of your application status. What is one way you could accomplish this within Azure?

- Enable the OMS portal that Azure provides. This operations management suite has the tools needed for log analytics.
- Enable Azure Log Analytics from the Azure Marketplace. Configure the activity logs and connect them to your application workspace.  ( Correct )
- Enable Azure Metrics. Configure Metrics to analyze the log files you need and import it into Azure Monitor.
- Enable a Container Monitoring solution from the Azure Marketplace. Configure its container to analyze your logs which can then be sent to Azure Monitor.

6. What query language does Azure Log Analytics use?

- HTSQL
- Adatis
- Kusto   ( Correct )
- Pl/SQL

7. Which of the following is a common practice for designing self healing systems in Azure?

- Embrace chaos engineering, which is intentionally injecting failures and abnormal conditions into your environment    ( Correct )
- Allow clients to send any number of unrestricted requests to your application, because it will automatically restart in the event of an error
- Run security scans for common encryption threats
- Only run self-heal testing in your lower environments to avoid restarting application instances in production

8. Why is it a good idea to set a size limit for crash dump files?

- Without a limit your application can encounter a stack overflow
- Crash dumps can be in the hundreds of megabytes making them difficult to parse and transfer.     ( Correct ) 
- Azure requires a limit otherwise your dumps will be truncated
- Setting a limit will allow Azure to log only the important critical failures.

9. What does the event tool in Azure Insights capture?

- How many sessions are in your application
- How often critical failures occur.
- How many people used your application
- How often pages and features in your application are used.    ( Correct )

10. Your application throws a common error when the system goes down and you want to be alerted when this occurs. However, you don't want thousands of alerts for the same issue. How can you prevent that from happening?

- Use a new pipeline for alerts that only messages developers when the application healthcheck fails.
- Send errors to a database and send an alert only once a common error is thrown hundreds of times.
- Use Smart Groups to generate alerts that encapsulate related alerts to reduce alert noise.     ( Correct )
- Create an Azure dashboard to aggregate common errors and subscriber notifications for your development team to this dashboard.

11. The Azure Test and Feedback can be used in both Azure DevOps and what other system?

- Github
- Apache Subversion
- JIRA
- Azure DevOps Server 2019    ( Correct )

12. Which could be determined by using the Metrics Explorer?

- The count of a certain event     ( Correct )
- The latency for all users of your application
- The latest release timestamp for your application
- The reason for a bug in your application

13. How could you split a telemetry metric in a chart by property within Azure Insights?

- Change the metric aggregation type to "Unique."
- Change the metric aggregation to "Count."
- Turn Grouping On and pick a property.     ( Correct )
- Create two metrics for the properties.

14. What Azure Monitor application could you use to create interactive dashboards?

- User Flows
- Workbooks   ( Correct )
- Impact
- Retention

15. What shell environment could you use to manage and configure VMs in Azure?

- Azure Cloud Shell     ( Correct )
- Azure CLI
- Azure CMD
- Azure Bash

16. How might Azure Storage benefit your production application ow mWhat purpose could using Azure Storage have for your production application?

- Allows for inexpensive archival of application log data    ( Correct )
- Allows for relational application logs with fast query compatibility
- Allows for real-time updates of system outages
- Allows visibility into changes to your Azure infrastructure

17. You want your application to have the ability to collect user feedback so that the development team can make updates according to user preferences. How can you implement this?

- Integrate HockeyApp with your application to collect in-app feedback.    ( Correct )
- Create a new Azure pipeline for collecting feedback.
- Allow users access to the database to provide direct feedback.
- Code a serverless function in Azure for collection user feedback.

18. You are routing sensitive crash data that often contains information on public critical infrastructure within Azure. You are not allowed to transmit data over public internet. How would you route this data back to an on-prem infrastructure to meet these requirements?

- Use a message queue in Azure that contains encrypted packets of data that the on-prem server can read
- Utilize IPVanish to enable end-to-end secure transfers and to secure your critical data.
- Utilize ExpressVPN to enable end-to-end secure transfers and to secure your critical data.
- Utilize ExpressRoute to enable end-to-end secure transfers and to secure your critical data.    ( Correct )

