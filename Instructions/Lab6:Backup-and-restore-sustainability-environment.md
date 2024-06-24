# Lab 5 - Backup and Restore Sustainability Environment (Read Only)

## Lab Overview

In this lab, you will learn how to protect and restore your data within the Microsoft Power Platform and Dataverse. This includes understanding the types of backups available, the retention periods for different environment types, and the steps to perform manual and system backups. You will also learn how to extend backup retention periods and restore data effectively, ensuring continuous availability of service and compliance with data protection standards in a sustainability context.

## Lab Scenario

As an administrator responsible for maintaining the sustainability initiatives within your organization, you must ensure that all data related to sustainability is adequately backed up and can be restored in case of any data loss or system failure. This lab will guide you through the process of creating backups, extending retention periods, and restoring data using the Power Platform admin center and PowerShell.

## Lab Objectives

By the end of this lab, you will be able to:

1. Understand the types of backups (system and manual) and their retention periods.
2. Create manual backups before major customizations or updates.
3. Change the backup retention period for production environments without Dynamics 365 applications using PowerShell.
4. Restore system backups to ensure data availability and integrity.

## Exercise 1: Understand Backup Types and Retention Periods

### Task 1: Review Backup Types and Retention Periods

In this task, you will review the different types of backups available in the Microsoft Power Platform and their corresponding retention periods.

1. System backups:
   - Created automatically for environments with a database.
   - Retention periods vary based on environment type.

2. Manual backups:
   - Initiated by users before major customizations or updates.
   - Retention periods depend on whether the environment has Dynamics 365 applications.

      | Environment types                          | System backup | Manual backup |
      |--------------------------------------------|---------------|---------------|
      | Production with Dynamics 365 apps          | 28 days       | 28 days       |
      | Production without Dynamics 365 apps       | 7 days        | 7 days        |
      | Sandbox                                    | 7 days        | 7 days        |
      | Developer                                  | 7 days        | 7 days        |
      | Teams                                      | 7 days        | 7 days        |
      | Default                                    | 7 days        | Not supported |
      | Trial                                      | Not backed up | Not supported |
      | Trial (subscription-based)                 | Not backed up | Not supported |

## Exercise 2: Create Manual Backups

### Task 1: Create a Manual Backup

In this task, you will create a manual backup of a sustainability-related environment.

1. Sign in to the Power Platform admin center using administrator credentials.
2. Navigate to **Environments**, select an environment, and then select **Backup & Restore > Create a backup**.
3. Enter a name and description for the backup.
4. Select **Create** and wait for the backup to complete.

## Exercise 3: Change Backup Retention Period

### Task 1: Extend Backup Retention Period Using PowerShell

In this task, you will use PowerShell to extend the backup retention period for a production environment that doesn't have Dynamics 365 applications.

1. Prepare your environment for PowerShell by installing the PowerShell for Power Platform Administrators module.
2. Run the following PowerShell command to set the retention period:

    ```powershell
    Set-AdminPowerAppEnvironmentBackupRetentionPeriod -EnvironmentName "Environment ID" -NewBackupRetentionPeriodInDays 28
    ```

3. Verify the retention period using:

    ```powershell
    Get-AdminPowerAppEnvironment -EnvironmentName "Environment ID"
    ```

## Exercise 4: Restore System Backups

### Task 1: Restore a System Backup

In this task, you will restore a system backup to ensure data recovery and continuity.

1. Sign in to the Power Platform admin center using administrator credentials.
2. Navigate to **Environments**, select an environment, and then select **Backup & Restore > Restore or manage**.
3. On the **System** tab, select a backup date and time.
4. Click **Continue**.
5. Select a target environment (must be a sandbox environment) and then select **Restore**.
6. Confirm that you want to overwrite the environment.

## Review

### Key Takeaways

- **Types of Backups:** You have learned about system and manual backups, their differences, and their retention periods.
- **Creating Backups:** You have successfully created manual backups to safeguard data before making significant changes.
- **Retention Period Management:** You have extended the backup retention period for production environments using PowerShell.
- **Restoring Data:** You have restored system backups to ensure data recovery and continuity.

By completing these exercises, you have gained practical skills in managing backups and restoring data in the Microsoft Power Platform, ensuring the protection and availability of sustainability-related data.
