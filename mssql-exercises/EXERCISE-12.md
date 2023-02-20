##  <a id="exercise12">Exercise 12 - Create and Save a Hook Operation Template

In this exercise, you will:

  * Create a Hook Operation Template called: _CREATE APPUSER_

  * Insert code into the template that will create a Login and database user named _appuser_
  
Hook operations allow users to execute custom operations at select points during linking sources and managing virtual datasets.

**Steps**

1. Create a new Hook Operation Template called: Create APPUSER

  1. Click on the **Manage** menu

  2. Click on Hook Templates

2. Click on Plus sign

  2. Name - CREATE APPUSER

  3. Type - Powershell Script

  4. Contents (enter exactly - opening the lab in the lab server and copy/pasting this is highly recommended):

   ```
    [System.Reflection.Assembly]::LoadWithPartialName('Microsoft.SqlServer.SMO')
    $sqlserver = "."
    $dbname = $env:VDB_DATABASE_NAME
    $name = "appuser"
    $Server = New-Object ('Microsoft.SqlServer.Management.Smo.Server') $sqlserver
    if (-Not $Server.Logins.Contains($name))
    {
    $Login = New-Object -TypeName Microsoft.SqlServer.Management.Smo.Login -ArgumentList $Server, $name
    $Login.LoginType = 'SqlLogin'
    $Login.Create('delphix')
    }
    $database = $server.Databases["$dbname"]
    $user = new-object ('Microsoft.SqlServer.Management.Smo.User') $database, $name
    $user.Login = $name
    $user.Create()
   ```
---|---

**IMPORTANT:** Make sure the carriage returns you see here are the same in the pasted contents.

![images/download/attachments/90015915/worddav776c4bc8f6c814c302fb74e649b7599b.png](images/download/attachments/90015915/worddav776c4bc8f6c814c302fb74e649b7599b.png)

  2. Click Create

  3. Click Close

  [Back to MS SQL Lab Guide](/README.md) | [Back to Workshop Guide](../README.md)