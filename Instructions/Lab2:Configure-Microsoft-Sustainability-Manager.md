# Lab 2: Configure Microsoft Sustainability Manager 


### Task 1: Prepare Business Units and Hierarchy  

In this task, you will set up the Company profile, hierarchy, and facilities for the Wide World Importers organization in Microsoft Sustainability Manager.

1. In the left navigation pane, Select **Company profile** under **Settings** .

1. The Company profile page includes basic information about the organization, such as name, address, company logo, the annual reporting period, and relevant industries. Additionally, there are tabs at the top of the page for setting up organization structure and facilities, both will be covered in this exercise.

   ![image](./Images/Lab01/image10.svg)

1. On the **Company profile** page, select the **Industries** tab. Microsoft Sustainability Manager includes a selection of pre-defined industries and sub-verticals based on NACE standards, see NACE Code at https://nacev2.com/en. Select **+Add**.

   ![image](./Images/Lab01/image11.svg)

   ![image](./Images/Lab01/image12.svg)

1. Select **Transportation and storage**.

    ![image](./Images/Lab01/image13.svg)

1. In the next screen, select **Land transport and transport via pipelines** and select **Add**.

    ![image](./Images/Lab01/image14.svg)

1. **Land transport and transport via pipelines** is now visible in the **Industries** section at the bottom of the **Company profile** page.

    ![image](./Images/Lab01/image15.svg)

1. In the **Company profile** page, switch to the **Structure** tab.

  ![image](./Images/Lab01/image16.svg)


9. Select **Contoso USA** and select **Add** to add a new organizational unit under it.

    ![image](./Images/Lab01/image17.svg)


10. Enter the following data for organizational unit and select **Save** in the button pane:

    1. **Name**: Wide World Importers
    1. **Organizational unit type**: Department

   ![image](./Images/Lab01/image18.svg)


11. In the **Organizational hierarchies** section, which appears after selecting **Save**, select **+ New Organizational hierarchy**.

    ![image](./Images/Lab01/image19.svg)


12. Set the following values and select **Save & Close**:

    1. **Parent**: Contoso USA
    1. **Effective start date**: The first day of the current month (MM/DD/YYYY)

    ![image](./Images/Lab01/image20.svg)

13. After being returned to the **Organizational Unit**, select **Save & Close** to return to the **Company profile**.

    ![image](./Images/Lab01/image21.svg)

14. If necessary, navigate to **Company profile**, switch to the **Facilities** tab page and select **Add facility**.

  ![image](./Images/Lab01/image22.svg)

15. Create a new Facility with the following details. Once the values are entered, select **Save & Close**:

    >[!NOTE] **Note:** Pay close attention to the data used in this lab. The following labs will reference this data, and it will need to match exactly as seen in the lab.

    1. **Name**: Wide World Importers - Miami Office
    1. **Address line 1**: Brickell Avenue
    1. **City**: Miami
    1. **State**: Florida
    1. **Zip**: 33132
    1. **Country**: United states of America
    1. **Latitude**: 25.774320
    1. **Longitude**: -80.187720

    >[!NOTE] **Note:** Latitude and Longitude are not required but are used to display a pin on the Facilities map. They can be automatically added by selecting an address from the autocomplete options in Address line 1, or manually entered.

    ![image](./Images/Lab01/image23.svg)

16. Using the same steps, add another new **Facility**. Once the values are entered, select **Save & Close**.

    >[!NOTE] **Note:** Pay close attention to the data used in this lab. The following labs will reference this data, and it will need to match exactly as seen in the lab.

    1. **Name**: Wide World Importers - Tampa Office
    1. **Address line 1**: Lois Avenue
    1. **City**: Tampa
    1. **State**: Florida
    1. **Zip**: 33609
    1. **Country**: United states of America
    1. **Latitude**: 27.944830
    1. **Longitude**: -82.514050


**Note:** Latitude and Longitude are not required but are used to display a pin on the Facilities map. They can be automatically added by selecting an address from the autocomplete options in Address line 1, or manually entered.

![image](./Images/Lab01/image24.svg)


Great job, by completing these steps, you have assisted Alex with completing the organizational setup in Microsoft Sustainability Manager for Wide World of Importers. This included the Company profile, hierarchy, and facilities. Organizational structure and facility management will be linked to activity and emission data to group emissions by Organization, facility, and even regions. This is an important part of carbon emission reporting and organization disclosures. **Please continue to the next task.**



## Task 2: Setup reference data

In this task, Reed sets up the reference data for contractual instrument types in Microsoft Sustainability Manager. Contractual instrument types are the different types of contractual agreements that a firm has with their providers and suppliers.


1. Navigate to **Reference data** on the left side of the page under **Data**.


1. Select **Contractual instrument types** and select **View**.

    ![image](./Images/Lab01/image27.svg)


1. Under **Active contractual instrument types**, select **New** to create new contractual types.

    ![image](./Images/Lab01/image28.svg)


1. Create a new Contractual Instrument with the following details. Once entered, select **Save & Close** in the button pane.

    1. **Name**: VanArsdel Ltd
    1. **Energy source**: Nuclear

    **Note:** Pay close attention to the data used in this lab. The following labs will reference this data, and it will need to match exactly as seen in the lab.

   ![image](./Images/Lab01/image29.svg)


1. In the same way, again create a new Contractual Instrument with the following details. Once entered, select **Save & Close** in the button pane.

    1. **Name**: Adatum Corp
    1. **Energy source**: Other

   ![image](./Images/Lab01/image30.svg)


    **Note:** Pay close attention to the data used in this lab. The following labs will reference this data, and it will need to match exactly as seen in the lab.

Great job, by completing these steps, you have helped Reed add reference data for contractual instrument types. There are many types of reference data. Take some time after this lab to explore the other reference data types. They will be used throughout Microsoft Cloud for Sustainability, and Microsoft Sustainability Manager. **Please continue to the next task.**



## Task 3: Setup Unit conversion factor

In this task, Reed sets up a unit conversion factor in Microsoft Sustainability Manager. While reviewing the inventory management plan, Alex identifies a missing unit of distance needed to calculate emissions for the fleet of electric vehicles. They ask Reed to add a new unit to the Length/Distance unit group.

Unit Groups are used to group units together and define a base unit used to convert between unit types. For example, the Length/Distance unit group contains units of length and distance, with a base unit of meter (m). The units within the Length/Distance unit group have conversions between the unit type and meter, such as miles convert to 1,609.344 meters. You can explore this functionality in deeper detail on Microsoft Docs, please visit **Set up unit groups** at https://docs.microsoft.com/en-us/industry/sustainability/setup-unit-groups.

1. Navigate to **Unit groups** on the left side of the page under **Settings > Applications.**


1. Under **Active unit groups**, select **Length/distance** and open it.

   ![image](./Images/Lab01/image32.svg)


1. Select **New unit** to create a new unit.

   ![image](./Images/Lab01/image33.svg)


1. Enter the following details to create a new unit. Once entered, select **Save & Close** from the button pane.

    1. **Name**: 100 mile
    1. **Conversion factor**: 160934.40

**Note:** The EPA calculates electric vehicle efficiency by the number of kilowatt hours (kWh) used per 100 miles. For consistency, it is best practice to utilize the same

![image](./Images/Lab01/image34.svg)


Great job, by completing these steps you have helped Reed add the missing unit for the fleet for elctric vehicles to the Length/Distance unit group to Microsoft Sustainability Manager.

## Task 4 : Create a reporting year 

Alex and Reed will set up the reporting years in Microsoft Sustainability Manager. Alex will name the reporting year, set up the start date and use a template to create more than one period. 

**Note:** The Reporting years you set up will override the configuration in General settings.

Alex proceeds to create a reporting year in Sustainability Manager. For detailed information, see Configure reporting years 

1.	In the left navigation pane, under **Settings**, select **Company** **profile**. Select the **Reporting years** tab.

   ![image](./Images/Lab01/image35.svg)
 
2.	Select **Create reporting year.**

  ![image](./Images/Lab01/image36.svg)

 
3.	Enter the following details. After you've entered the values, select **Save**. 

  	a.	**Name** - Enter Fiscal – 2022.  This name appears on the **Insights** page in Microsoft Sustainability Manager.

  	b.	**Start date**: 01/01/2022.  

  	c.	**Year template** - Annual.

       ![image](./Images/Lab01/image37.svg)

 
4. Select **Close**. The reporting year will generate with the first period starting on the **Start date** and the last period ending one year from the **Start date**.


![image](./Images/Lab01/image38.svg)

**Congratulations!** Alex and Reed of Wide World Importers now have their organizational structure set up along with the contractual instrument types, and a new unit in the Length/Distance unit group. This forms the foundation for the rest of the work they will do with the Microsoft Cloud for Sustainability and Microsoft Sustainability Manager. These data points are used throughout the tools, so it is important to spend the time to ensure that your organization and reference data is set up correctly.
