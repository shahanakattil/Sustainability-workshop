# Lab 4: Using Reporting

## Overview

In the previous lab, the ingested Activity data was taken through calculation designs using calculation models and the output was reviewed in terms of CO<sub>2</sub>E unit. In this lab, we will perform a set of activities to generate emissions reports, activity reports, and review Power BI dashboards.

Finally, this lab will help us gain insights into the emission activity trends and identify the opportunities to set scorecards and carbon reduction goals that are detailed in the next lab.


###  Lab Scenarios

In this lab, Amber Rodriguez – Sustainability specialist for Contoso Corp reviews the data in the Insights section of Microsoft Sustainability Manager, noticing that Wide World Importers was a large contributor to Scope 2 emissions in 2022. Amber informs Jessie Irwin - Sustainability lead for Contoso Corp that the Activity and Emission Reports are available for review. Jessie opens the reporting section and creates a new Activity report and a new Emissions report. Jessie reviews the generated report and includes the report in the sustainability reporting procedures for Contoso Corp.


### Learning Objectives

In this lab, you will do the following:

-  Executive Dashboard  

-  Emission Insights 

-  Waste Insights 

-  Other Reporting 

### Prerequisites

-   Microsoft Sustainability manager environment is set up with sample data
-   Lab 1 organization and reference data is entered
-   Lab 2 activity data is ingested
-   Lab 3 emissions are calculated

### Solution Focus Area

Analytics reports present calculated emissions in an organized way to detect trends and perform further exploration of data. These reports are updated soon (within approximately 30 minutes) after the calculations are run and allow the users to review the outcome of calculations in an aggregated format. Data can also be exported in predefined report formats that include groupings for emissions and activity, and other dimensions. These formats can be used to do deeper analysis and prepare many different types of reports.

![image](./Images/Lab04/image1.svg)

In this lab exercise, we will focus on the scenarios illustrated below:

![image](./Images/Lab04/image3.svg)

## Exercise 1: Sustainability Dashboards

In this exercise, you will take on the persona of Amber Rodriguez – Sustainability Specialist for Contoso Corp. utilizing the various Sustainability Dashboards to gain insights into the organization.

1. Log into the virtual machine using the virtual machine credentials located on the **Resources** tab above.

2. Open a new browser window and navigate to https://make.powerapps.com.

3. Log into your Microsoft 365 tenant using the credentials for the tenant located on the **Resources** tab above.

4. If needed, change the environment to your trial on the top bar.

5. Open the **Sustainability Manager** Application by clickin on Play button.

**Important** Please make sure that you have completed the previous labs to ensure that the dashboards and reports show meaningful data.

## Task 1 :  Executive dashboard

1. The Executive dashboard in Microsoft Sustainability Manager provides an overview of total emissions, revenue intensity, and renewable energy categorized by scope, geography, organizational unit, and facility.

     ![](../media/report1.png)

2. You can filter this dashboard by Reporting year, Accounting method, and Organizational hierarchy. Under Filters select **Fiscal -2022** then **Organizational hierarchy** expand **Contoso Corp** > **Contoso USA** then select check box next to **Wide World Importers**. 

    ![](../media/report2.png)

3. The options for Accounting method include:

    - Location Based: Reflects the average emissions intensity of grids on which energy consumption occurs.
    - Market Based: Reflects emissions from electricity you purposefully chose.
    - The tiles at the top of the dashboard let you quickly assess the following metrics:

        a). Emissions: Total emissions, together with a breakdown by scope 1, scope 2, and scope 3.

        b). Revenue intensity: Revenue intensity score, together with a breakdown by scope 1, scope 2, and scope 3. (Revenue intensity equals emissions divided by revenue.)

        c). Renewable energy (%): Renewable energy as a percentage of total energy, together with a breakdown by renewable energy source.

4. You can review the option by **By country / region**, **By organization unit** and  **By facility**. 
    
    ![](../media/report3.png)

## View trends

The bottom tile has three tabs that show a graphical representation of emissions, revenue intensity score, renewable energy, and water production intensity.

Emissions: This tab has a toggle that lets you view either total emissions in a trend line chart or emissions by scope. Emissions by scope appear in column charts for the three scopes that show emissions over time.

Revenue intensity score: This tab has a toggle that lets you view either revenue intensity in a trend line chart or revenue intensity categorized by scope. Revenue intensity by scope appears in column charts for the three scopes that show emissions over time.

Renewable energy: This tab has a toggle that lets you view either renewable energy as a percentage in a column chart over time or renewable energy breakdown by source. Renewable by source data appears in a column chart for each source showing the percentage of renewable energy as a percentage of total energy over time.

Water production intensity: This tab shows values for water production intensity consumed, discharged, and withdrawn. Water production intensity is the total amount of water used in relation to the total weight of products produced.


### Task 2: Explore Emission Insights 

In this task, Amber explores the various **Sustainability** dashboards which provide an overview of total emissions, revenue intensity, and renewable energy broken down by scope, geography, organizational unit, and facility.

1.  In the left navigation pane, under **Analytics**, select **Emission Insights.**

2.  Select **Insights** on the left pane.

3.  The page displays the **Emissions overview** dashboard, the dashboard is filtered by selecting a reporting period and accounting method. The top tile in the dashboard has four tabs: All emissions, By month (comparison), By scope, and By scope (line chart). The first, third, and fourth tabs have a toggle that is used to **Show a comparison by year**. When the toggle is off, data for the selected reporting period is shown in a monthly view. When the toggle is on, all available years are shown on a trend chart. The details around each of the tabs in the top tile are as follows:

    -   (1) All emissions – This tab shows total emissions over time.
    -   (2) By month - This tab shows a breakdown of emissions by month for the selected reporting period.
    -   (3) By scope – This tab shows a breakdown of emissions by scope 1, scope 2, and scope 3. It includes a chart for each scope.
    -   (4) By scope (line chart) – This tab shows each scope as a separate line on one chart. Therefore, you can easily compare emissions by scope over time.
    -   (5) The **By source and scope** tile at the bottom shows a further breakdown of data in each scope. It shows specific sources and their contribution to emissions overall.
    -   (6) The tile at the bottom right has three tabs: **By country/region**, **By organizational unit**, and **By facility**. Each tab shows a breakdown of emissions by scope 1, scope 2, and scope 3.
    -   (7) Select **2022** under **Filters : Reporting period** on the left side to explore the data. **Note**: The data in the image below may not match your data.

4.  Select **Scope 1** on the top tab to view the Scope 1 emissions dashboard. Scope 1 emissions are emissions that are owned or directly controlled by the organization. Like the Emissions overview, the **Scope 1 emissions** dashboard lets users view scope 1 emissions by reporting period.

    (1) Summary statistics can be viewed in the left tile. These statistics include the total scope 1 emissions for the current reporting period compared to the previous period. They also include emissions by source type and emissions broken down by greenhouse emissions. Greenhouse emissions include the following gases:

    -   **CO<sub>2</sub>** – Carbon dioxide
    -   **CH<sub>4</sub>** – Methane
    -   **N<sub>2</sub>O** – Nitrous oxide
    -   **HFCs** – Hydrofluorocarbons (that is, manufactured compounds that contain hydrogen and fluorine atoms)
    -   **PFCs** – Perfluorocarbons (that is, manufactured compounds that contain carbon and fluorine atoms)
    -   **NF<sub>3</sub>** – Nitrogen trifluoride
    -   **SF<sub>6</sub>** – Sulfur hexafluoride

    (2) The top tile has four tabs: **Scope 1 emissions**, **By month (comparison), **By source**, and **By source (line chart)**. The first, third, and fourth tabs have a toggle that is used to **Show a comparison by year**. When the toggle is off, data for the selected reporting period is shown in a monthly view. When the toggle is on, data for all reporting periods is shown on a trend chart.

    (3) The bottom-left tile provides a deeper dive into the source of the scope 1 emissions by category. It has a tab for each category of scope 1 emissions:

    -   **Stationary combustion** – This category includes emissions from electricity, heat, steam, or energy to power industrial or commercial uses. The tab shows emissions by fuel type.
    -   **Mobile combustion** – This category includes emissions from cars, trucks, and other motor vehicles; boats and other water vessels; locomotives; and aircraft. The tab shows emissions by vehicle type.
    -   **Industrial processes** – This category includes emissions from various non-energy-related industrial events or manufacturing activities, or from consumers. The tab shows emissions by process type.
    -   **Fugitive emissions** – This category includes emissions that were accidentally released into the atmosphere. These emissions include gases and vapors. The tab shows emissions by activity type.

    (4) The bottom-right tile has three tabs: **By country/region**, **By organizational unit**, and **By facility**. Each tab shows scope 1 emissions for the corresponding delineation of data.

5.  Select **Scope 2** on the top tab to view the Scope 2 emissions dashboard. Scope 2 are emissions that a company causes indirectly when the energy it purchases and uses. For example, for Wide World electric fleet vehicles the emissions from the generation of the electricity they're powered by would fall into this category. Just as with other dashboards, the **Scope 2 emissions** dashboard lets users view scope 2 emissions by reporting period and accounting method.

    (1) The summary statistics can be viewed in the left tile. These statistics include the total scope 2 emissions for the selected reporting period compared to the previous period. They also include scope 2 emissions by source. Scope 2 emissions have the following sources:

    -   Purchased heat
    -   Purchased cooling
    -   Purchased electricity
    -   Purchased steam

    (2) The top tile has four tabs: **Scope 2 emissions**, **By month (comparison), **By source**, and **By source (line chart)**. The first, third, and fourth tabs have a toggle that is used to **Show a comparison by year**. When the toggle is off, data for the reporting period is shown in a monthly view. When the toggle is on, data is shown for all available reporting periods.

    (3) The bottom tile has three tabs: **By country/region**, **By organizational unit**, and **By facility**. Each tab shows scope 2 emissions for the corresponding delineation of data.


6.  Select **Scope 3** on the top tab to view the Scope 3 emissions dashboard. Scope 3 emissions are the result of activities from assets not owned or controlled by the reporting organization, but that the organization indirectly impacts its value chain. Scope 3 emissions include all sources not within an organization's scope 1 and 2 boundary. The **Scope 3 emissions** dashboard in Microsoft Sustainability Manager lets you view scope 3 emissions by reporting period.

    (1) Summary statistics can be viewed in the left tile. These statistics include the total scope 3 emissions for the reporting period compared to the previous period. The tile also shows all categories of scope 3 emissions classified as either upstream or downstream. Scope 3 emissions have the following fifteen categories.

    **Upstream**

    -   Purchased Goods and Services
    -   Capital Goods
    -   Fuel and energy related activities
    -   Upstream transportation and distribution
    -   Waste generated in operations
    -   Business travel
    -   Employee commuting
    -   Upstream leased assets

    **Downstream**

    -   Downstream transportation and distribution
    -   Processing of sold products
    -   Use of sold products
    -   End-of-life treatment of sold products
    -   Downstream leased assets
    -   Franchises
    -   Investments

    (2) The top tile has four tabs: **Scope 3 emissions**, **By month (comparison), **By category**, and **By category (line chart)**. The first, third, and fourth tabs have a toggle that is used to **Show a comparison by year**. When the toggle is off, data for the selected reporting period is shown in a monthly view. When the toggle is on, the data that is shown represents all available reporting periods.

    (3) The bottom-left tile has five tabs:

    -   **By category** – This tab shows scope 3 emissions by category and type.
    -   **By leased assets** – This tab shows the number of records and emissions by upstream and downstream leased assets.
    -   **By facility type** – This tab shows the number of records and emissions by type of facility.
    -   **By supplier** - This tab shows the number of records and emissions by supplier.
    -   **By waste** – This tab shows the number of records and emissions by waste.

    (4)The bottom-right tile has three tabs: **By country/region**, **By organizational unit**, and **By facility**. Each tab shows scope 3 emissions for the corresponding delineation of data.

7.  Select **Renewable energy** on the top tab to view the summary view of renewable energy, its sources, and the contract type.

    (1) The summary statistics can be viewed in the left tile. These statistics include renewable energy as a total percentage of energy that was used for the selected reporting period compared to the previous period. The tile also shows the percentage of renewable energy by source type, such as solar, wind, and water.

    (2) This tile has three tabs: **Renewable energy**, **By source**, and **By source (line chart)**. Each tab has a toggle that you can use to show a comparison by year. When the toggle is off, data for the selected reporting period is shown in a monthly view. When the toggle is on, data is shown for all reporting periods.

    (3) The bottom-left tile shows renewable energy by contract type. It indicates the renewable energy in the appropriate measure, such as kilowatt-hour (kWh), and the percentage of renewable energy.

    (4) The bottom-right tile has three tabs: **By country/region**, **By organizational unit**, and **By facility**. Each tab shows renewable energy for the corresponding delineation of data.

8.  Select **Deep analysis** on the top tab to dive deeper into data and uncover insights that might not be available from other reports. The dashboard can be filtered by selecting a reporting period and accounting method.

    The **Decomposition tree** can be used to drill down from the company-level to more granular levels of the organization, and to access:

    -  High value
    -  Low value
    -  Emission source
    -  Country/region
    -  Organization
    -  Different levels of scope 1, scope 2, and scope 3 emissions.
    -  Facility

9.  Amber drills into our decomposition tree to identify where our high sources of emissions are. Select the **+** next to **Total emissions**, and select **Scope**. (Images may not match displayed data.)

10.  Amber can see which scope has the largest volume of emissions. Select the **+** next to **Scope 2**, and select **Emission source** to identify which Scope 2 emission source is biggest contributor.


11.  It seems that Purchased electricity was the biggest contributor of emissions. Select the **+** next to **Purchased electricity** and select **Country/region** to identify which regions were contributing to the large Purchased electricity emissions.

12.  The USA contributed the most to the Purchased Electricity emissions. The Country/Region selection is driven by the country region mapping table found in the Settings area. Select the **+** next to **USA** and select **Organization** to see which organizations contributed to this.

13.  You can see the organizations with the largest to lowest contributor to Contoso Corp’s carbon emissions

14. In further filtering we see the Wide World Importers under Org level 3. Use this information to create a goal for Wide World Importers to reduce their Purchased electricity emissions by 300 mtCO2E (you'll complete this task in the next exercise).

16.	Select **Custom Dimensions** tab to view the emission analytics

     •	You can view a time chart of CO2E emissions broken by custom dimension strings. For example, compare emissions by vehicle size where Vehicle Size is a custom dimension with string value.
     
     •	Expand the tree view of total CO2E emissions and drill into each string custom dimension present in the data and view CO2E emissions by value.
     
     •	Explore the time chart of CO2E emissions intensity broken out by custom dimension strings, where the intensity denominator is a numeric custom dimension, you select. 
     
     •	Expand the tree view of total CO2E emission intensity, where the intensity denominator is a numeric custom dimension, you select. You can drill into each string custom dimension in the data and view CO2E emission intensity associated with each unique string value.
 
You've now successfully explored various Sustainability dashboards. You can use these dashboards to gain insights into your emissions data. Additionally, as you drilled down from total emissions to the organization level, you were able to determine that Wide World Importers needs to reduce the carbon emissions from purchased electricity. This goal could be achieved in a variety of ways, such as switching to renewable energy sources or using more energy-efficient devices and vehicles. You can use these insights to drive business decisions and then use the information to create scorecards and goals to track your progress.

Great job, you have successfully explored various Sustainability dashboards with Amber to gain insights into the emissions data. You can see as you drilled down from total emissions to the organization level, Amber was able to determine that Wide World Importers needs to reduce the carbon emissions from Purchased electricity. This could be achieved in a variety of ways such as switching to renewable energy sources or using more energy efficient devices and vehicles. You and she can use these insights to drive business decisions and use the information to create scorecards and goals to track progress. **Please continue to the next task.**

## Task 3 :  Waste Insights

1. The Water insights dashboard in Microsoft Sustainability Manager provides you with a holistic view of your organization's water sustainability performance relative to the business. Based on the selected water transaction type, the tiles contain the following information about your organization:

    - Water revenue intensity (total water quantity/total revenue)
    - Water production intensity (total water quantity/total weight of products produced)
    - To open the Water insights dashboard in Sustainability Manager, select Analytics on the left navigation, and then select Water insights.

1. Select the Water insights tab.

1. Filter the dashboard by water transaction type, water stressed area, reporting period, or organizational hierarchy.

1.  Water quality dashboard
The Water quality dashboard in Microsoft Sustainability Manager lets you view your organization’s water quality related data at a facility or organizational unit level by reporting period. These water quality transactions primarily consist of the quality information in waste water discharges from facilities.

1.  Waste quantity dashboard
The Waste quantity dashboard in Microsoft Sustainability Manager provides a view of your organization’s waste quantity data. It shows total waste generated by diversion method, hazardous and radioactive waste type at a facility, or organizational unit level for the reporting period.

1. Circularity (Input material) dashboard (preview)

1. The Circularity (Input material) dashboard (preview) in Microsoft Sustainability Manager provides you with a view of the circular practices implemented during the inflow of materials into your organization.

1. The dashboard shows the quantity of component items used and the percentage of sustainable content such as renewability, reusability, and recyclability present in these items for each finished good. You can further filter by packaging material or reporting period.

1. Circularity (Finished good) dashboard (preview)

1. The Circularity (Finished good) dashboard (preview) in Microsoft Sustainability Manager provides you with a view of the circular design principles implemented in final finished products. The dashboard shows the total quantity and the percentage of finished goods following circularity design principles.

1. The Circularity (Finished good) dashboard includes the following two tiles:

1. Follows circularity design principle

   - To view the corresponding charts for each of these tiles, select one of these tabs:

          All quantity
          By month
          By finished good (weight)
          By finished good (percentage)


## Task 4:  Generate Quantitative preparation report

In this exercise, Amber Rodriguez informs Jessie Irwin - Sustainability lead for Contoso Corp that the Activity and Emission Reports are available for review. Jessie generates quantitative preparation reports that extract emission and activity data from Microsoft Sustainability Manager. The reports are in an Excel format that can be used to submit the data for public disclosure.

1.  In the left navigation pane, select **Reporting**.

2.  Select **New**.

     ![](../media/report5.png)

3.  Set the following fields:

    1. **Report type**: Emissions report
    1.  **Name**: MC4S Emissions report
    1.  **Report type**: Emissions report
    1.  **Start date**: 01/01/2022
    1.  **End date**: 12/31/2022

    Fields can be selected to group data by, or column headers for the report. The available fields for Emissions report are **Country/Region**, **Regional group**, **Latitude/Longitude**, **Organization unit**, **Facility**, **Is market based**, **Is biogenic**, **Scope**, **Emission source**, **Activity type**. (The **Organization hierarchy date** field appears only after the **Organization unit** field is selected.).

4. For this task, Jessie will just set the following fields to **Yes** for use in Contoso Corp’s carbon emissions reporting for public disclosure:

    - **Country/Region**
    - **Regional group**
    - **Facility**
    - **Scope**
    - **Emissions source**
    - **Activity data** 

     ![](../media/report6.png)
    
5. Once these are selected, select **Save & Close** on the top command bar.

6.  Once the report is saved, the **Generate report** button will be visible on the command bar. Select **Generate report** and then the report is queued to be generated.

       ![](../media/report7.png)
  
7.  Select **Refresh** button on the command bar until the **Report generation status** is changed from **Pending** to **Ready for download.** This may take a few minutes to generate.

     ![](../media/report8.png)

8.  Once the status is changed, a **Download report** button is visible in the command bar. Select that button to download the generated report. An Excel report begins to be downloaded. Open the report.

     ![](../media/report9.png)

10.  The reports contain the following information:
    - The **Group by** column headers that were selected. In this case, it is grouped by Country/Region, Regional group, Facility, Scope, Emissions source, and Activity type
    - The following emission metrics: **CO<sub>2</sub>**, **CH<sub>4</sub>**, **N<sub>2</sub>O**, **SF<sub>6</sub>**, **NF<sub>3</sub>**, **CO<sub>2</sub>E**, **HFCs**, **PFCs**, and **Other GHGs.**

Great job, you have helped Jessie successfully generate an emissions report. Emissions reports are useful for providing information in public disclosures. Microsoft Sustainability provides this information in a tabular format to allow you to adapt it to meet the rapidly changing regulatory requirements. There is a great opportunity for partners to assist in the generation of the disclosure documents by configuring an emissions report to export data in a consistent and familiar format for ingestion into a partner solution. This report can be used in conjunction with the activity report, which will be generated in the next task. **Please continue to the next task.**


## Sustainability scorecards and goals

Scorecards and Goals allow organizations to monitor progress against data-driven goals. They can help you curate sustainability metrics and track them against your company's key business objectives. After you’ve created a scorecard that includes some goals, you can periodically check on the scorecard’s progress and make required adjustments.

Additionally, you can have manual goals with the ability to connect to data and set rules for automatic status updates. You can enable several scorecards and goals and subgoals.

Scorecards and goals are manually updated or connected to data for automatic check-ins with optional Microsoft Teams collaboration.

### Scorecards


1. When goals are connected to data, the service will run periodically and manage updates.

1. The status updates can be data-driven and dynamic, and they’ll continue to adjust if you connect goals to data and set rules to determine the status as data is collected. You can compare the goals and progress on the Scorecards page.

### Goals

1. Review the details of the goal. As you review the details of the goal, you can add notes to record your observations. This step is useful for stakeholders when they’re reviewing goals to help understand why they might be behind and to inform them of what they should do next.

1. You can use the Microsoft Teams for collaboration and chat feature to allow primary Sustainability Manager users, such as facility managers to CFOs, to collaborate with anyone who contributes to sustainability goals. This feature allows stakeholders to communicate and make decisions about data or insights.

1. The Microsoft Teams integration feature also tracks and stores the conversation in context for ease of reference later. The integration feature is built on Microsoft Dynamics 365 capabilities, and it was made available in preview when Microsoft Sustainability Manager was released in GA (general availability).

1. You can enable the Microsoft Teams integration feature in Settings. You can also select the type of records for which you want to enable Teams collaboration, such as the Emissions data record.

1. To initiate a conversation, create a new linked chat, find the team member that you want to contact, and then add a message.

1. This record will be tracked in Teams, so whenever you open a linked record, the conversation will be available. All participants have access to the specific record in context.

**Congratulations!** Amber is now comfortable using the dashboards to gain insights into the emissions data. She can use these insights to drive business decisions and use the information to create scorecards and goals to track progress. In addition, Jessie can now build the emission and activity reports and include them in the sustainability reporting procedures for Contoso Corp. These reports will help develop goals that can be tracked using Scorecards, which will be created in the next lab.