# Lab 3: Import Sustainability Data 

### Learning Objectives

In this lab, you will do the following:

-   Use Microsoft Sustainability Manager connectors to ingest data
-   Use Power Query to transform the data before ingestion
-   Review the ingested data in the “Purchase Electricity Activity Data” Dataverse Table
-   The newly ingested activity data during this lab exercise will be utilized in the remaining scenarios (calculations and reporting) in the upcoming lab exercises.

### Solution Focus Area

In this lab, the focus is on the “Data Ingestion” aspect of the Solution Focus Area. It follows the “Organization and Reference data Set up” and forms the basis for the emission calculations and the reporting thereafter. The Microsoft Sustainability Manager is flexible with multiple automated options to ingest data – such as the connectors as well as manual inputs. For scenarios that may require complex data transformation and/or ETL, tools like Azure Data Factory are recommended. You can explore this functionality in deeper detail on Microsoft Docs at **Overview of Microsoft Cloud for Sustainability Data Import**, https://docs.microsoft.com/en-us/industry/sustainability/import-data.

### Scenario

In this lab, Reed Flores – IT Admin for Wide World Importers utilizes the activity data Excel spreadsheets sourced by Alex Serra – Emissions Analyst. The Activity data spreadsheets contain Electricity Purchased for the year 2022 and Miles driven by the fleet of Fabrikam Electric Trucks for the calendar year 2022. Reed observes that associated information such as product, model and Vehicle size needs to be added as custom dimension meta data before importing which are required to run the emission calculation and gather the Emission insights reports for monitoring. After adding this information, Reed uses Microsoft Sustainability Manger’s connector functionality to import from the Excel spreadsheets, and reviews other connectors available for future purposes. Reed uses the built-in Power Query functionality to transform the data to match Microsoft Sustainability Manager’s data schema and looks for other potential issues such as case-sensitive d data fields.


## Exercise 1: Import Data

In this exercise, you will learn about the steps that Reed takes to ingest the spreadsheets given by Alex. Data import is a vital task to bringing large volumes of data into Microsoft Sustainability Manager. Excel is utilized in this lab; however, many pre-built connectors are available, and Partners can build custom connectors to integrate with additional data sources. You can explore this functionality in deeper detail on Microsoft Docs, please visit **Overview of data connectors** at https://docs.microsoft.com/en-us/industry/sustainability/import-data-connectors.

**Important** Please ensure you have completed the previous lab to create Reference Data. **The data import process requires all Reference Data to exist, and the process is case sensitive, so please ensure the Reference data that was added has the exact same case formatting as what is found in the lab**. Failure to do so will result in errors during the data import process

1. Log into the virtual machine using the virtual machine credentials located on the **Resources** tab above.

1. Open a new browser window and navigate to `https://make.powerapps.com`.
 
1. Log into your Microsoft 365 tenant using the credentials for the tenant located on the **Resources** tab above.

1. If needed, change the environment to your trial on the top bar.

2. For this exercise, you'll use OneDrive.

   Ensure that your personal OneDrive has been initialized by selecting the app selector button in the upper-left corner of the screen.

  	![image](../media/ima1.png)

3. Select OneDrive from the Apps list.
   
   ![image](../media/ima2.png)

5. A tab with your new OneDrive will open. Close this tab and return to Power Apps.

   ![image](../media/ima3.png)

1. Open the **Sustainability Manager** Application by clicking on Play button.

    You will land on the **Home** page for Microsoft Sustainability Manager.

    ![image](../media/ima4.png)


### Task 1: Add custom dimension metadata

In this task, Reed will add additional information to the Excel spreadsheet that Alex provided: **Purchased electricity Wide World Importers 2022.xlsx**. Reed will add custom dimensions metadata for the mapping before importing the data from the Excel spreadsheet. 

 
3.	Select the **Custom dimensions** tab under **Data**.
     
 
4.	Select **New** on the top right on the Active Custom dimensions page.

   ![image](../media/ima5.png)
 
5.	Enter the details as follows: 

  	 1. Logical name - Product
   
     2. Display name – Product

     3. Description - Product (This is optional)
  	
      4. Click **Save & Close**.

    ![image](../media/ima6.png)
 
6.	Repeat the previous steps to create another custom dimension metadata as follows 

      •	Logical name - Model
      
      •	Display name - Model
      
      •	Logical name - Vehicle Size  
      
      •	Display name – Vehicle Size
      
       ![image](../media/ima7.png)

### Task 1: Import 2022 data for “Purchased Electricity“ for Facilities

In this task, Reed imports the Excel spreadsheet provided by Alex, _Purchased electricity Wide World Importers 2022.xlsx_. This brings in the Electricity Purchased by Wide World Importers facilities for the year 2022 into the Purchased electricity activity data.

1.  In the left navigation pane, under **Data**, select **Imports** and select **New**
   
5. On the **Imports**, select **POWER QUERY GUIDED EXPERIENCE**.

   ![image](../media/ima8.png)
 
6. Under **Carbon activities**, Select **Add**, next to **Purchased electricity** under Category name

    ![image](../media/ima9.png)
 
7. Select **Next**.
   
8. Review the large list of connectors by selecting the **Excel workbook**, as the Data source.
 
    ![image](../media/ima10.png)

9. A new dialog will open for Power Query. Select the **Upload file** option and then select **Browse**.

    ![image](../media/ima11.png)
    
    Note - You can also choose to import an existing file that's located in OneDrive. For simplicity of this exercise, you'll use the Upload file functionality.
 
10. On the file selection window, browse to the location of the Excel files that were downloaded.
    
    1.	Select the **Purchased electricity Wide World Importers 2022.xlsx file**.

    2.	Select **Open**.

    ![image](../media/ima12.png)
 
11. After the file has successfully uploaded, you might be required to select **Sign in** to create a new connection credential.

    ![image](../media/ima13.png)
 
12. An Office 365 Sign-in dialog will appear. Reed will select their user from the list. In this exercise, select your  user account from the list.

13. After the sign-in process is complete, the new connection will be selected automatically. Select **Next**.

     **Note** - If you receive an error after uploading the Excel file, check your browser cookie settings.

14. On the Choose data page of the Power Query wizard:

    1. Select the **Purchased electricity** Excel spreadsheet.

    2. Select **Transform data**.

       ![image](../media/ima14.png)

15. You can complete various data and column transformations on the **Transform data** page of the Power Query wizard. As a result, you can adjust data types, update column mappings, and perform advanced transformations that you're familiar with in Microsoft Power Platform dataflows or Microsoft Power BI datasets. For this exercise, do not apply any transformations, click **Create**.

**Note** - Wait for the transformations to be applied properly, before you click **Create**, else you may get an error.

   ![image](../media/ima15.png)
    
16. The **New data connection** wizard will now be on the **Schedule data** **import** page, where you'll complete the following actions:

     1. Turn on the **Import data automatically** toggle to allow the option to set a schedule for the data to be imported automatically. Selecting this     
        option is beneficial if the connector will be used in a scenario where the data will change frequently, such as a web API or FTP server.

      2. Turn on the **Replace previously imported data** toggle to remove all previously imported data and bring in the full dataset that was retrieved. 
         Selecting this option is beneficial if the data source isn't providing data from only the last import or if it always includes a full set of data. For 
         this scenario of importing historical data, leave both options turned off.
    
17. Select **Next** when finished.

      ![image](../media/ima16.png)
 
18. On the Review and finish page, complete the following tasks:
    
    1. Enter a name for the new connection, such as **Wide World Importers Purchased Electricity 2022**

    2. Select **Connect**.

    ![image](../media/ima17.png)
 
19. Next, you'll need to map your source data to the data model. Data will not appear until this step is complete. Select on **Map fields**.

      ![image](../media/ima18.png)
 
20. Select the **Data source** to map, in this exercise select **Purchased electricity** under **Carbon Activities.**

     ![image](../media/ima19.png)
 
21. In this scenario, Reed will need to map the columns from the spreadsheet to the columns in Microsoft Sustainability Manager. Select **Auto Map** for the solution to automatically map the file’s source fields with the destination fields, for any field that is not an exact match the best match will be found and highlighted in blue, make sure to review them. Review the custom dimensions to ensure Model and Product are added as part of mapping. Remove the unnecessary custom dimensions if they are added When you are done with the mapping, select **Save**.

      ![image](../media/ima20.png)

       ![image](../media/ima21.png)

23. Now that we have reviewed our field mappings, toggle **Ready to Import** as yes. Click the back arrow. Click on **Done**.

     ![image](../media/ima22.png)

     ![image](../media/ima23.png)
 
24. You will be navigated back to **Data imports** where you can view the import you created.

25. The **Data Import** job will run, and the status will display **Scheduled** and then in a moment it switches to **Processing**. You might need to refresh your page to view the change.

26. After a minute or two select **Refresh** above the list to view the updated status, which should be **Complete**.
 
     ![image](../media/ima24.png)
 
27. Go to **Carbon Activities** on the left navigation pane under **Data management**.

28. Find **Purchased electricity** in the **Scope 2: Indirect emissions** section and then select **View**.

      ![image](../media/ima25.png)
 
The Purchased electricity view shows all purchased electricity activity data that has been imported.

   ![image](../media/ima26.png)
 
28. Filter the view by selecting the **Organizational Unit** dropdown menu and then selecting **Filter By**.

29. Select **Wide World Importers** from the **Filter By** dialog.

30. Select **Apply** to apply the filter to the column.

     ![image](../media/ima27.png)
 
After a few moments, the view will refresh and the activity data records that were imported during this exercise will be displayed.

 ![image](../media/ima28.png)

You've now completed the data import of 2022 Purchased Electricity for Wide World Importers. This step is imperative in realizing the goal of recording, reporting, and reducing carbon emissions. Next, you'll import the 2022 Miles Driven for Wide World Importers fleet of electric vehicles.


