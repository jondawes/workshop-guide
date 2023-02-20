##  <a id="exercise2"></a>Exercise 2 - Configure the DB User on the Source

In this exercise, you will:

* Connect to the Windows Source
* Configure domain user privileges
* Configure the local Delphix user

### Steps

1. Double click "RDP" icon on the Student Desktop
2. Double click "Windows Source" icon
3. Login as the delphix_src user (login details are in the **Getting Started** section of this guide)
4. On the Windows Source machine, go to Start -> All Programs -> Microsoft SQL Server 2008 R2 -> SQL Server Management Studio

_Note: You may need to scroll down on the right-hand side of the RDP window to
see the Windows Start button or expand the screen_.

![images/download/attachments/90015915/worddav1bc729235b8002f7001e71f93f5bb657.png](images/download/attachments/90015915/worddav1bc729235b8002f7001e71f93f5bb657.png)

  * Under Authentication, select "SQL Server Authentication"
  * Log in as sa/delphix

![images/download/attachments/90015915/worddav6bdc70f2145e7449d5af927b4aade4f7.png](images/download/attachments/90015915/worddav6bdc70f2145e7449d5af927b4aade4f7.png)

5. Configure the domain user privileges
  * Expand the Security folder, then Logins
  * Double Click on DELPHIX\delphix_src
  * Click on "User Mapping"
  * Check the box next to "master"
  * Select "db_datareader" for the database role membership
  * Click OK
  
![images/download/attachments/90015915/worddavdab58dcd241bf78681ef20fd35fb29ca.png](images/download/attachments/90015915/worddavdab58dcd241bf78681ef20fd35fb29ca.png)

6. Right click Logins
7. Select New Login
8. Fill in the following details on the General Screen:
  * Login Name: delphix_db
  * SQL Server Authentication
  * Password: delphix
  * Unclick "Enforce password expiration"
  * Unclick "User must change password at next login"
  * On the left, click "User Mapping"
  * Check master, then select "db_datareader" from the role list

![images/download/attachments/90015915/worddav6aa444b271c421ba92d8494df29c80e6.png](images/download/attachments/90015915/worddav6aa444b271c421ba92d8494df29c80e6.png)

  * Check msdb, then select "db_datareader" from the role list

![images/download/attachments/90015915/worddavae5eb8a15a987ee4539e6bbfc7ede08d.png](images/download/attachments/90015915/worddavae5eb8a15a987ee4539e6bbfc7ede08d.png)

  * Check AdventureWorks2008R2, then select "db_backupoperator" from the role list to allow copy only full backups

![images/download/attachments/90015915/worddavee9552067446e2d322be3c53ec4cb20f.png](images/download/attachments/90015915/worddavee9552067446e2d322be3c53ec4cb20f.png)

  * Click OK

[Back to MS SQL Lab Guide](/README.md) | [Back to Workshop Guide](../README.md)