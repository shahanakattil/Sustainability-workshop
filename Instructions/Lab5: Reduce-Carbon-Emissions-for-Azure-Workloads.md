## Review an existing Azure deployment

Content not found

## Connect to MSM 
Content not found

## Review actions to optimize the carbon emissions.  
Content not found

## Emission Impact Dashboard for Azure 

## Install the app

2. Select the following link to get to the app: Emissions Impact Dashboard template app.

3. On the AppSource page for the app, select GET IT NOW.

    ![](../media/appsource.png)

4. When prompted, select Install.

   ![](../media/install-app.png)

5. When the app finishes installing, it appears on your Power BI Apps page. Select the app and open it.

   ![](../media/app-on-app-page.png)

6. Select Connect your data.

   ![](../media/connect-your-data.png)

8. In the Connect to Emissions Impact Dashboard dialog that appears, under EnrollmentIDorBillingAccountID, enter either your billing account ID (formerly known as the enrollment number) for EA Direct customers or billing account ID for MCA/MPA.

    ![](../media/connect-enterprise-agreement.png)
   When done, select Next.

10. Connect your account:

      For Authentication method, select OAuth2.
      For Privacy level setting for this data source, select Organizational.
      When done, select Sign in and connect.

   ![](../media/authentication-dialog.png)
   
9. Select the user account. Be sure to sign in with the credentials that have access to the enrollmentID/Billing AccountID with valid permissions as explained in the prerequisites.

10. Wait for the view to build, which can take up to 24 hours. Refresh the dataset after 24 hours.

## Update the app
Periodically you might receive update notifications from Appsource/Power BI about a new version of the app. When you install the new version, the following options are available:    

Select Update the workspace and the app, and then select Install. The update installs, overwriting the existing/installed workspace and app.

## Issues

If there are any issues with the dataset refresh/app update during the updating process, validate these steps and refresh the dataset.

Follow these steps to make sure your dataset configurations are set correctly:

1. Go to the workspace panel and open the app workspace.

2. Open the Scheduled Refresh option in the dataset settings and make sure the billing account ID is correct.

    ![](../media/schedule-refresh.png)

3. Open the Parameters section and configure the data source again in the Data Source section with the credentials that have access to the Enrollment ID / Billing Account ID with valid permissions, mentioned in the prerequisites.

   ![](../media/data-source-credentials-parameters.png)

4. After the above steps are validated, go back to the app workspace and select the Refresh option.

   ![](../media/data-refresh.png)

5. After the dataset refreshes successfully, select the Update App option at the top-right corner of the app workspace.

   ![](../media/updating-app.png)


## Review Emission Impact Dashboard for M365 
