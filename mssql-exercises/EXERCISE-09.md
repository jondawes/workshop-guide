## <a id="exercise9">Exercise 9 - Refresh a VDB

In this exercise, you will:

  * Create a new table on your source database

  * Snapshot the dSource

  * Refresh your VDB - devdb

  * Verify the new table appears on the VDB

VDBs can get out of sync as new data comes into the source system. Refreshing a VDB will re-provision it from the dSource. Refreshing a VDB will delete any changes that have been made to it over time.

**Steps**

1. Log into the Source via RDP

2. Go to Start -> All Programs -> Microsoft SQL Server 2008 R2 -> SQL Server Management Studio

  1. Under Authentication, select "SQL Server Authentication"

  2. Log in as sa/delphix

3. Expand "Databases"

4. Right click AdventureWorks2008R2, then select New Query

5. Run the following command (by clicking **Execute**):

_select * into sourcetab_ _from
AdventureWorks2008R2.HumanResources.vEmployee;_

  1. Take a transaction log backup, by right-clicking the **AdventureWorks2008R2** folder, selecting **Tasks** and **Back Up**, and then choose Backup Type = "Transaction Log."

![images/download/attachments/90015915/worddava5a77e557a0072bcfa9542d42a5b36c6.png](images/download/attachments/90015915/worddava5a77e557a0072bcfa9542d42a5b36c6.png)

  1. Go back to the Delphix Engine GUI

  2. Within a couple of minutes a new timecard will appear for the dSource

![images/download/attachments/90015915/worddavc66064a49de61163934a9d1167ea0bc6.png](images/download/attachments/90015915/worddavc66064a49de61163934a9d1167ea0bc6.png)

  1. Select the _devdb_ VDB and click the _Refresh_ button

![images/download/attachments/90015915/worddav5dbe8a0de8c6119dee9f219da2f3e034.png](images/download/attachments/90015915/worddav5dbe8a0de8c6119dee9f219da2f3e034.png)

  1. Refresh the _devdb_ VDB using the latest snapshot from the AdventureWorks2008R2 dSource

![images/download/attachments/90015915/worddav04258906537af6dfaccf142d87ec7bfc.png](images/download/attachments/90015915/worddav04258906537af6dfaccf142d87ec7bfc.png)

  1. Click Submit button

Once the refresh has completed, you can log into _devdb_ to confirm.

  1. Log into the Target via RDP

  2. Go to Start -> All Programs -> Microsoft SQL Server 2008 R2 -> SQL Server Management Studio

    1. Under Authentication, select "SQL Server Authentication"

    2. Log in as sa/delphix

  3. Expand "Databases"

  4. Right click devdb, then select New Query

  5. Run the following command:

_select count(*) from_ _sourcetab;_

If this returns a count of rows, the snapshot/refresh was successful.

[Back to MS SQL Lab Guide](/README.md) | [Back to Workshop Guide](../README.md)