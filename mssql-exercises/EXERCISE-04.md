## <a id="exercise4"></a>Exercise 4 - Configure the Windows Target/Staging Server

In this exercise, you will:

  * Download the Delphix Connector
  * Install the Delphix Connector
  * Enable Powershell scripts on the target

Before we start this exercise is important to mention that in Delphix, a
Target and Staging server have the same configuration. It's a Delphix best
practice to isolate the Staging workload from the VDB workload, so that's why
it has a different name, but from a requirements point of view, they
are the same.

### Steps

1. Double click "RDP" icon on the Student Desktop
2. Double click "Windows Target" to connect to the Windows Target server
3. Login as the delphix_trgt user (login details are in the **Getting Started** section of this guide)
4. Open Google Chrome from your Windows Target desktop
5. Navigate to your Delphix Engine at 10.0.x.10 ('x' is your **Student Number** )
  * Log in as the delphix_admin user
  * Go to Manage -> Environments
  * Click the ellipses (…) and select _Add Environment_

![images/download/attachments/90015915/worddava57004a26ec15405b106bc030428200a.png](images/download/attachments/90015915/worddava57004a26ec15405b106bc030428200a.png)

  On the _Host and Server_ tab choose **Windows** as the _Host OS_ and **Target** as the _Host Type_ then click Next

![images/download/attachments/90015915/worddav8207f96e2ec2346bb3593fca6d19d381.png](images/download/attachments/90015915/worddav8207f96e2ec2346bb3593fca6d19d381.png)

  Click the " _Download Delphix Connector Installer_ "

  ![images/download/attachments/90015915/worddav2cec493c04282a0948d461830f63e148.png](images/download/attachments/90015915/worddav2cec493c04282a0948d461830f63e148.png)

  Once it finishes downloading, click Keep

6. Open Windows Explorer and go to Downloads
7. Double click on DelphixConnectorInstaller
   * Click "Run"
   * Click "Next"
   * Agree to the terms and conditions and click Next
   * Accept the default Connector Port of 9100 by clicking Next
   * Accept the default location of C:\Program Files\Delphix\DelphixConnector\ by pressing Next. (Note: you do not need to fill this in, it will auto-populate on the next screen after you press next)
   * Click Next to install
   * Click Yes to allow the installation when the User Account Control (UAC) dialog pops up
   * Once it finishes, click Close
8. Go to Start -> All Programs -> Accessories -> Windows PowerShell
9. Right click on Windows PowerShell and select Run as Administrator

![images/download/attachments/90015915/worddav37d0d98713699f10eccf388f0fa0efcd.png](images/download/attachments/90015915/worddav37d0d98713699f10eccf388f0fa0efcd.png)

10. Click Yes to run with elevated privileges
11. Type: _Set-ExecutionPolicy Unrestricted_ at the Powershell prompt
12. Press "Y" and enter

![images/download/attachments/90015915/worddav415115917b3a7248c896f65fd5e67a0a.png](images/download/attachments/90015915/worddav415115917b3a7248c896f65fd5e67a0a.png)

[Back to MS SQL Lab Guide](../README.md) | [Back to Workshop Guide](/README.md)