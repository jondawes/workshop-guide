## <a id="exercise14">Exercise 14 - Recovering a deleted table using log sync

  * Create a table

  * Delete the table

  * Backup transaction log

  * Recover the table from transaction log(log sync)

**Steps**

1. Create a table as follows on source server
  _select * into Logsync_tab from AdventureWorks2008R2.HumanResources.vEmployee;_
(  Note the time  )

2. Wait for few minutes (to give time for the table to be created)

3. Drop the table called **Logsync_tab** and note the time.

  `drop table Logsync_tab;`

4. Take a transaction log backup (right-click on AdventureWorks2008R2 folder, click Tasks --> Back Up, and select Transaction Log from the dropdown labeled "Backup Type")

5. Wait until the dSource Timeflow reflects this Transaction log time

6. Create a VDB by selecting date and time from the Timeflow

Choose the transaction log prior to latest log (Latest log is the log that has
create and drop table actions).
![images/download/attachments/90015915/worddav5e4ee402d32c897fd7e2fb7945d31400.png](images/download/attachments/90015915/worddav5e4ee402d32c897fd7e2fb7945d31400.png)

7. Expand the log by clicking on "Open LogSync" (second icon)

![images/download/attachments/90015915/worddavb724a7df4d69bcc36f8720602c26756b.png](images/download/attachments/90015915/worddavb724a7df4d69bcc36f8720602c26756b.png)

8. Change the date time to the time after the table creation

![images/download/attachments/90015915/worddave970119b2523181f35ef86d47d09389a.png](images/download/attachments/90015915/worddave970119b2523181f35ef86d47d09389a.png)

9. Create VDB by clicking on "provision VDB "(First icon). Name the VDB -  RecoverTable

![images/download/attachments/90015915/worddav93cd80cb066e616d4d371544566a1b88.png](images/download/attachments/90015915/worddav93cd80cb066e616d4d371544566a1b88.png)

10. After the VDB is created, look for the table on target server.

* Log into the Target via RDP

* Click Start and go to SQL Server Management Studio

* Click Connect to log in as delphix\delphix_trgt

* Expand Databases

* Expand the " RecoverTable " virtual database

[Back to MS SQL Lab Guide](/README.md) | [Back to Workshop Guide](../README.md)