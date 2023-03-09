# <a id="exercise7">Exercise 7 - Add the dSource
In this exercise, you will:

  * Add the 'AdventureWorks2008R2' dSource into Delphix and bring in the initial backup

With an environment set up, users can then sync databases into Delphix. The Delphix engine will read the source database and create a dSource (a custom object). The dSource is not a functional image of the database but a storage-efficient object from which virtual databases can be created. When creating a dSource, Delphix will pull over the complete dataset using standard database protocols. Subsequent sync operations, as governed by user-defined policies, will pull only incremental changes.

### Steps

1. Navigate to Manage -> Datasets
![images/download/attachments/90015915/worddav9e7bebc06f9b20af064be6f7cfee8f08.png](images/download/attachments/90015915/worddav9e7bebc06f9b20af064be6f7cfee8f08.png)

2. Click the Plus ![images/s/en_GB/7104/0e21dd459285e7b3b5e0deaa2193b2af8bbb7c8b/_/images/icons/emoticons/add.png](images/s/en_GB/7104/0e21dd459285e7b3b5e0deaa2193b2af8bbb7c8b/_/images/icons/emoticons/add.png) and choose Add dSource from the drop-down

![images/download/attachments/90015915/worddav2958c211ddad293eda939aee9835b88b.png](images/download/attachments/90015915/worddav2958c211ddad293eda939aee9835b88b.png)

3. On the Add dSource wizard, review the information and pre-requisites on the Preparation tab then click Next

4. On the Source tab click the **AdventureWorks2008R2** Data Source to select it and enter the information below

  1. Environment User: **delphix\delphix_src**

  2. Select the **Database User** radio button

  3. Database Username: **delphix_db**

  4. Database Password: **delphix**

5. Click **Validate**

![images/download/attachments/90015915/worddav8bb0df9f181973de20b59b9d42146c90.png](images/download/attachments/90015915/worddav8bb0df9f181973de20b59b9d42146c90.png)

  1. Click Next

  2. Click the "Add Dataset Group" link

  3. Enter the Group Name: MS SQL Databases

![images/download/attachments/90015915/worddave772fb62eb64e16a9377455a00dd0751.png](images/download/attachments/90015915/worddave772fb62eb64e16a9377455a00dd0751.png)

  1. Click OK and select the new group in the list

  2. Click Next

  3. Select "Use the most recent full or differential backup"

  4. For Backup Path, enter: \\\10.0.x.50\Backups ('x' is your **Student Number** )

  5. For Staging Environment, select WINTARGET

  6. For Validated Sync Mode, select Transaction log backups and click Enabled next to LogSync

![images/download/attachments/90015915/worddavc65a9f8c30a092fd185f8798cadb5538.png](images/download/attachments/90015915/worddavc65a9f8c30a092fd185f8798cadb5538.png)

  1. Click Next

  2. Click Next

  3. Verify your settings and click Submit

![images/download/attachments/90015915/worddav7a7c7a2bfdf971568f777ebdb65cc8f0.png](images/download/attachments/90015915/worddav7a7c7a2bfdf971568f777ebdb65cc8f0.png)

  1. Go to the main Delphix page by clicking Delphix in the top left corner of the GUI

  2. Monitor the AdventureWorks dSource addition via the progress bar and the Actions pane

[Back to MS SQL Lab Guide](/README.md) | [Back to Workshop Guide](../README.md)
