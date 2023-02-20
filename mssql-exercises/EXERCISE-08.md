##  <a id="exercise8">Exercise 8 - Provision a VDB

In this exercise, you will:

  * Create a VDB called _devdb_

  * Log into the VDB

The objective of Delphix virtualization is to provide easy access to virtualized databases (VDBs) that resemble production and other data systems. VDBs are fully functional database images that can be created from dSources.

**Steps**

1. Click the AdventureWorks2008R2 dSource in the MS SQL Databases group

2. Select the most recent snapshot and click Provision

![images/download/attachments/90015915/worddav3085f064e4f8ef634a3e6b842d9d7a0b.png](images/download/attachments/90015915/worddav3085f064e4f8ef634a3e6b842d9d7a0b.png)

3. Select WINTARGET on the left pane of the wizard and click Next.

![images/download/attachments/90015915/worddav7a064602a7e50c005324835caf52ca23.png](images/download/attachments/90015915/worddav7a064602a7e50c005324835caf52ca23.png)

4. Enter the Database Name: devdb

5. Click Next

![images/download/attachments/90015915/worddavb3b0808308ca79137738934d4a716d26.png](images/download/attachments/90015915/worddavb3b0808308ca79137738934d4a716d26.png)

6. Select the dataset group "MS SQL Databases group"

7. Click Next

8. Keep the defaults values for retention and click Next

9. Keep the defaults for hooks and click Next

10. Verify settings and click Submit

![images/download/attachments/90015915/worddavedaf9dd2350c832578b57088bdf5261c.png](images/download/attachments/90015915/worddavedaf9dd2350c832578b57088bdf5261c.png)

![images/download/attachments/90015915/worddavd168a0bfbee6ce0b7c49ad670fae3cfd.png](images/download/attachments/90015915/worddavd168a0bfbee6ce0b7c49ad670fae3cfd.png)

It may take a couple minutes for the VDB creation to complete. You can monitor
the progress on the left hand side of the screen next to the _devdb_ object in
the MS SQL Databases group. On the _Actions_ pane on the right hand side of
the screen, you should see the _Provision virtual database "devdb"_ item move
to the _Recently completed_ pane without error. Once the VDB is created, you
can verify that the VDB is operational by:

1. Log into the Target via RDP

2. Click Start and go to SQL Server Management Studio

3. Click Connect to log in as delphix\delphix_trgt

4. Expand Databases

5. Note the "devdb" virtual database

6. Note the validated sync database (named with a GUID)

![images/download/attachments/90015915/worddavb25e4fbd60b085d4fe46430358b42272.png](images/download/attachments/90015915/worddavb25e4fbd60b085d4fe46430358b42272.png)

[Back to MS SQL Lab Guide](/README.md) | [Back to Workshop Guide](../README.md)