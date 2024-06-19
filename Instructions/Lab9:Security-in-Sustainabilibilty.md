# Lab 09 - Security in Sustainability

## Lab overview
In the initial phase of setting up the security infrastructure, the focus is on creating essential components to monitor and analyze security events. This involves establishing a Log Analytics workspace and integrating Microsoft Sentinel into the workspace, laying the foundation for subsequent security measures.

## Lab scenario
In this lab, you will undertake the essential task of setting up Log Analytics, which provides a centralized location to store and query data, while Sentinel serves as the platform for advanced security analysis, also enabling proactive threat detection and incident response.


## Excercise 1 - Setup Sentinel Workspace

### Task 1: Create Sentinel Workspace

In this task, you will create Microsoft Sentinel workspace where you will be monitoring and analyzing security events in upcoming labs.

1.  On Azure Portal page, in **Search resources, services and docs (G+/)** box at the top of the portal, enter **Microsoft Sentinel**, and then select **Microsoft Sentinel** under services.

    ![Picture 1](../media/l9.1.png)

1. From the Microsoft Sentinel page, select **+ Create**.

1. From Add Microsoft Sentinel to a workspace, select **+ Create a new workspace**.

1. From the basics tab of the Create Log Analytics workspace, enter the following and click **Review + Create**.   

    | Setting | Action |
    | -- | -- |
    | Subscription |  Retain the default Subscription.  |
    | Resource group | select **sustainability** |
    | Name | Set the name to **sustainabilityworkspace**. |
    | Region | Retain the default region. |
    |||

    ![Picture 1](../media/l9.2.png)

1. Verify the information you entered then select **Create**.

1. If you don’t see the new workspace listed, select **Refresh**, then select newly created workspace **sentinelworkspace** and click on **Add**.

1. Once the new workspace is added, the Microsoft Sentinel | News & guides page will display., including that the Microsoft Sentinel free trial is activated. Select **OK**  Note the three steps listed on the Get started page.

   ![Picture 1](../media/image_8.png)
   
   ![Picture 1](../media/image_9.png)

## Excercise 2 - Ingest Logs from Microsoft Entra ID

### Task 1: Install Microsoft Entra ID data connector to Sentinel

In this task, you will explore the Microsoft Sentinel in the Azure Portal and install the Microsoft Entra ID data connector.

1. On Azure Portal page, in **Search resources, services and docs (G+/)** box at the top of the portal, enter **Microsoft Sentinel**, and then select **Microsoft Sentinel** under services.

     ![Picture 1](../media/l9.1.png)

1. Select **sentinelworkspace**.

1. Select the **Data Connectors(1)** under **Configuration** and select **Content hub(2)**.

     ![Picture 1](../media/l9.3.png)

1. Search and select the **Microsoft Entra ID** connector.

   ![Picture 1](../media/image_45.png)

1. Click on **Install**.

### Task 2: Set up the data connector to ingest logs to workspace

In this task, you will configure the Microsoft Entra ID data connector to ingest relevant logs into your designated Log Analytics workspace

1. In Microsoft Sentinel, select Data connectors.

1. Search for and select the **Microsoft Entra ID** connector.

1. In the details pane for the connector, select Open connector page.

1. On the **Instructions** page, under configuration, select the required record types data to be collected and click on **Apply changes**

   ![Picture 1](../media/l9.9.png)

  >**Note**: Wait for atleast 15 mins and proceed to next task.

### Task 3: View data ingested into Microsoft Sentinel

In this task, you will be checking the logs ingested to sentinel.

1. In Microsoft Sentinel, select Data connectors.

1. Search for and select the **Microsoft Entra ID** data connector.

1. In the details pane for the connector, select Open connector page.

1. Review the Status of the data connector. It should be Connected.

   ![Picture 1](../media/n785.png)   

1. Scroll down and select **Go to log analytics**.

1. In the query pane, run the default query, to view the activity data ingested into the workspace.

   ![Picture 1](../media/l9.8.png)   

  >**Note**: It might take upto **3hrs** to generate the activity logs.

# Excercise 3 - Ingest Logs from Dynamics365

### Task 1: Install Dynamics365 connector to Sentinel

In this task, you will explore the Microsoft Sentinel in the Azure Portal and install the Dynamics365 data connector.

1. On Azure Portal page, in **Search resources, services and docs (G+/)** box at the top of the portal, enter **Microsoft Sentinel**, and then select **Microsoft Sentinel** under services.

     ![Picture 1](../media/l9.1.png)

1. Select **sentinelworkspace**.

1. Select the **Data Connectors(1)** under **Configuration** and select **content hub(2)**.

     ![Picture 1](../media/l9.3.png)

1. Search and select the **Dynamics 365 - Connector Only** connector.

   ![Picture 1](../media/l9.4.png)

1. Click on **Install**.


### Task 2: Set up the data connector to ingest logs to workspace

In this task, you will configure the Dynamics365 data connector to ingest relevant logs into your designated Log Analytics workspace

1. In Microsoft Sentinel, select Data connectors.

1. Search for and select the **Dynamics 365** connector.

1. In the details pane for the connector, select Open connector page.

1. On the **Instructions** page, under configuration, click on **Connect**

  >**Note**: Wait for atleast 15 mins and proceed to next task.

### Task 3: View data ingested into Microsoft Sentinel

In this task, you will be checking the logs ingested to sentinel.

1. In Microsoft Sentinel, select Data connectors.

1. Search for and select the **Dynamics365** data connector.

1. In the details pane for the connector, select Open connector page.

1. Review the Status of the data connector. It should be Connected.

   ![Picture 1](../media/l9.5.png)   

1. Scroll down and select **Go to log analytics**.

1. In the query pane, run the default query, to view the activity data ingested into the workspace.

   ![Picture 1](../media/l9.6.png)   

  >**Note**: It might take upto **3hrs** to generate the activity logs.

1. In the query pane, run the below query, to view the in detail logs for Dynamics 365 activities.

```
Dynamics365Activity

```
   ![Picture 1](../media/l9.7.png)   

  >**Note**: It might take upto **3hrs** to generate the activity logs. 

Reference Link:
https://learn.microsoft.com/en-us/industry/sustainability/security-overview
