# <a id="exercise7">Exercise 7 - Add the dSource
In this exercise, you will:

  * Add the 'AdventureWorks2008R2' dSource into Delphix and bring in the initial backup

With an environment set up, users can then sync databases into Delphix. The Delphix engine will read the source database and create a dSource (a custom object). The dSource is not a functional image of the database but a storage-efficient object from which virtual databases can be created. When creating a dSource, Delphix will pull over the complete dataset using standard database protocols. Subsequent sync operations, as governed by user-defined policies, will pull only incremental changes.

### Steps

1. Navigate to **Manage -> Datasets**
2. Click on the **plus** after **Datasets** on the left part of the screen and click on **Add dSource** and click **Next** on the pop up screen
3. Review the information on the **Preparation** tab. We created our environments in the previous exercise but for the purposes of this lab we will skip creation of new policies.
4. Click **Next**
5. On the **Source** tab click **AdventureWorks2008R2** under the **Data Source** list
6. Enter the DB Username: _**delphix_db**_ with password: _**delphix**_
7. Click **Validate** Credentials
 
 ![image](https://user-images.githubusercontent.com/112052485/224075657-f6290169-41fa-4139-b400-e8237d4600d1.png)

 
8. Click **Next**
9. Click on **Add Dataset Group**
10. Enter the Group Name: _**MS SQL Databases**_
 
 ![image](https://user-images.githubusercontent.com/112052485/224076078-8f7673f9-4f86-4470-82bd-6c56750f6251.png)

 
11. Click **OK** and select the new group in the list
12. Click **Next**
13. Select **Use the most recent full or differential backup**
14. For **Backup Path**, Click the **pencil** and enter: _**\\\10.0.x.50\\Backups**_ (‘**x**’ is your **Student Number**)
15. For Validated Sync Mode, select **Transaction log backups** and click **Enabled** next to **LogSync**
16. For Staging Environment, select **WINTARGET**
17. Click **Next**
 
 ![image](https://user-images.githubusercontent.com/112052485/224078049-f605cc0e-20ae-4fef-b92d-2dc990c9a60f.png)

 
18. Accept the **Default Policies** and click **Next**
19. No **Hooks** will be used. Click **Next**
20. Review the **Summary** page and click **Submit** to start the **dSource creation process**
 
 ![image](https://user-images.githubusercontent.com/112052485/224078508-61eca947-35be-4a24-b8da-a552733d5f55.png)

  
21. Go to **Manage** -> **Datasets**
22. Monitor the **AdventureWorks** dSource addition via the progress bar and the **Actions** pane.
 

[Back to MS SQL Lab Guide](/README.md) | [Back to Workshop Guide](../README.md)
