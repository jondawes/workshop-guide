## <a id="exercise13">Exercise 13 - Provision a VDB with Hook Template

In this exercise, you will:

  * Create a VDB called qadb

  * Use the Hook Operation Template we created previously

  * Log into the Target Instance

  * Verify the Hook Operation Template was successful

**Steps**

1. Click the AdventureWorks2008R2 dSource in the MS SQL Databases group

2. Select the most recent snapshot and click the Provision icon

3. Select WINTARGET on the left pane of the wizard and click Next

4. Select the dataset group "MS SQL Databases group"

5. Enter the Database Name: qadb

6. Click Next to accept default policies

7. Click Next to proceed without masking

8. On the Hooks tab add a Configure Clone Hook (1. Click on the Plus sign. 2. Click on **Create from Template**)

![images/download/attachments/90015915/worddav38749211acfde4eff7ac3bf7655f8a59.png](images/download/attachments/90015915/worddav38749211acfde4eff7ac3bf7655f8a59.png)

9. On the Hook Operation dialog box, verify that _Configure Clone_ is selected for the Hook Point

10. Enter a name - APPUSER

11. Click Create

![images/download/attachments/90015915/worddav4582bd5da8fc427a3f271cfc84034e48.png](images/download/attachments/90015915/worddav4582bd5da8fc427a3f271cfc84034e48.png)

12. Verify settings and click Submit

![images/download/attachments/90015915/worddav3757b2259242a2385de9cf75736032ff.png](images/download/attachments/90015915/worddav3757b2259242a2385de9cf75736032ff.png)

It may take a couple minutes for the VDB creation to complete. You can monitor
the progress on the left hand
side of the screen next to the _qadb_ object in the MS SQL Databases group. On
the Actions pane on the right hand side of the screen, you should see the
Provision virtual database _qadb_ item move to the Recently completed pane
without error. Once the VDB is created, you can verify that the VDB is
operational by:

1. Log into the Target via RDP

2. Go to Start -> All Programs -> Microsoft SQL Server 2008 R2 -> SQL Server Management Studio

  1. Under Authentication, select "SQL Server Authentication"

  2. Log in as **appuser/delphix**

3. Expand "Databases"

4. Select qadb -> Security -> Users

This will verify that the VDB is online and that the APPUSER user was created
by our hook.

[Back to MS SQL Lab Guide](/README.md) | [Back to Workshop Guide](../README.md)