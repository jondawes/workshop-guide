## <a id="exercise3"></a>Exercise 3 - Take a Backup of the Source Database

In this exercise, you will:

  * Take a backup of the AdventureWorks2008R2 database
  * Verify the backup location share

### Steps

1. On the Windows Source machine, go to Start -> All Programs -> Microsoft SQL Server 2008 R2 -> SQL Server Management Studio
  * Under Authentication, select "SQL Server Authentication"
  * Log in as sa/delphix
2. Expand "Databases"
3. Right click AdventureWorks2008R2, then select Tasks -> Back Up...
4. Note the backup destination in C:\Backups and click OK

![images/download/attachments/90015915/worddav51f2df862ba552d46a1ef185ef61f657.png](images/download/attachments/90015915/worddav51f2df862ba552d46a1ef185ef61f657.png)

5. Click OK once the backup is complete
6. Open Windows Explorer and navigate to C:\
7. Right click "Backups" and select Properties
8. Select the Sharing tab
9. Click the "Share" button
10. Ensure the Delphix Source user is the Owner and Delphix Target user has read/write privileges

![images/download/attachments/90015915/worddavd6ca7fd647a60f9845420fe02b4e2b18.png](images/download/attachments/90015915/worddavd6ca7fd647a60f9845420fe02b4e2b18.png)

11. Click Cancel

[Back to MS SQL Lab Guide](../README.md) | [Back to Workshop Guide](/README.md)