# Lab 01 - Setup Sentinel Environment

## Lab overview
In the initial phase of setting up the security infrastructure, the focus is on creating essential components to monitor and analyze security events. This involves establishing a Log Analytics workspace and integrating Microsoft Sentinel into the workspace, laying the foundation for subsequent security measures.

## Lab scenario
In this lab, you will undertake the essential task of setting up Log Analytics, which provides a centralized location to store and query data, while Sentinel serves as the platform for advanced security analysis, also enabling proactive threat detection and incident response.

## Lab objectives
In this lab, you will complete the following tasks:
- Task 1: Create Sentinel Workspace

## Estimated timing: 30 minutes

## Architecture Diagram

  ![](../media/arch1.png)

### Task 1: Create Sentinel Workspace

In this task, you will create Microsoft Sentinel workspace where you will be monitoring and analyzing security events in upcoming labs.

1.  On Azure Portal page, in **Search resources, services and docs (G+/)** box at the top of the portal, enter **Microsoft Sentinel**, and then select **Microsoft Sentinel** under services.

    ![Picture 1](../media/image_7.png)

1. From the Microsoft Sentinel page, select **+ Create**.

1. From Add Microsoft Sentinel to a workspace, select **+ Create a new workspace**.

1. From the basics tab of the Create Log Analytics workspace, enter the following and click **Review + Create**.   

    | Setting | Action |
    | -- | -- |
    | Subscription |  Retain the default Subscription.  |
    | Resource group | select ResourceGroup(sentinel-rg). |
    | Name | Set the name to 'sentinelworkspace'. |
    | Region | Retain the default region. |
    |||

    ![Picture 1](../media/Log2.png)

1. Verify the information you entered then select **Create**.

1. If you don’t see the new workspace listed, select **Refresh**, then select newly created workspace **sentinelworkspace** and click on **Add**.

   ![Picture 1](../media/Log3t1.png)

1. Once the new workspace is added, the Microsoft Sentinel | News & guides page will display., including that the Microsoft Sentinel free trial is activated. Select **OK**  Note the three steps listed on the Get started page.

   ![Picture 1](../media/image_8.png)
   
   ![Picture 1](../media/image_9.png)

