# Lab : Monitoring and Logging

## Lab scenario


## Lab Overview

Monitoring and logging in a sustainability manager context, especially within Microsoft Cloud for Sustainability, involve tracking, managing, and analyzing data to ensure sustainable practices and compliance with environmental regulations. 

## Lab Objectives



## Execirse 1 : Monitoring and Logging


1. Login to https://admin.powerplatform.microsoft.com/ with following credentials:

   - **Email/Username:** <inject key="AzureAdUserEmail"></inject>
   - **Password:** <inject key="AzureAdUserPassword"></inject>

1. From the left navigation pane select **Environments** > **Sustainability Trial**.

   ![image](../media/lab01-142.png)
    
1. From the top menu bar select **Settings**.

   ![image](../media/lab01-143.png)

1. Expand **Audit and logs** then select **Audit settings**, under **Auditing** select check box next to **Start Auditing**, **Log access**  and **Read logs**.

   ![image](../media/lab01-144.png)

   ![image](../media/lab01-145.png) 

1. Back to **Settings** page, expand **Audit and logs** then select **Audit summary view** and review the data.

    ![image](../media/lab01-152.png)

    ![image](../media/lab01-153.png) 

1. Open another edge tab and beowser to https://compliance.microsoft.com/ then from the left navigation pane under solution select **Audit**.

    ![image](../media/lab01-146.png) 

1. Click on **Start recording user and admin activity** on **Audit** page.

     ![image](../media/lab01-151.png) 

1. On the **Audit** under **New search** tab specify the following:

    - select **Start date** and **End date** 
    - **Record Type** : **CRM** and **PowerPlatformAdministratorActivity**
    - User : Search and select  **<inject key="AzureAdUserEmail"></inject>**
    - Click on **Search**

       ![image](../media/lab01-147.png)

1. On the Audit Page refresh the page and monitor the status and wait until changes from **Queue > progress** to  **Completed**.

    ![image](../media/lab01-148.png)

    ![image](../media/lab01-149.png)

1. Then click on **Completed** link and you can view all the record

   ![image](../media/lab01-150.png)

   
