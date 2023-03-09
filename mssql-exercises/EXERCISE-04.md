## <a id="exercise4"></a>Exercise 4 - Configure the Windows Target/Staging Server

In this exercise, you will:

  * Download the Delphix Connector
  * Install the Delphix Connector
  * Enable Powershell scripts on the target

Before we start this exercise, it is important to mention that in Delphix, a
Target and Staging server have the same configuration. It's a Delphix best
practice to isolate the Staging workload from the VDB workload, so that's why we reference them separately. However, from a requirements point of view, they are the same.

### Steps

1. Double click **RDP** icon on the Student Desktop
2. Double click **Windows Target** to connect to the Windows Target server
3. Login as the _**delphix_trgt**_ user (login details are in the **Getting Started** section of this guide)
4. Open **Google Chrome** from your Windows Target desktop
5. Navigate to your **Delphix Engine** at 10.0.x.10 ('x' is your **Student Number** )
  * Log in as the _**admin**_ user
  * Go to **Manage -> Environments**
  * Click the ellipses (…) after **Environment** on the left-hand side of the screen and click on **Add Environment**
  * Click **Windows**,**Target** and **Standalone**
  * Click **Next**
  * Click **Download Delphix Connector Installer**
  * Once it finishes downloading, click **Keep**

   ![image](https://user-images.githubusercontent.com/112052485/224060881-31a356bd-ffd0-44a8-8c29-76b7f39cf917.png)


6. Open **Windows Explorer** and go to **Downloads** folder
7. Double click on **DelphixConnectorInstaller**
   * Click "Run"

   ![image](https://user-images.githubusercontent.com/112052485/224061589-d72de364-1141-4718-8cf0-f6048a61ff7e.png)

   
   * Click **Next**
   * Agree to the terms and conditions and click **Next**
   * Accept the default Connector Port of **9100** by clicking **Next**
   
   ![image](https://user-images.githubusercontent.com/112052485/224062104-52984024-0516-416c-ba34-dca0003b90aa.png)

   
   * Accept the default location of **C:\Program Files\Delphix\DelphixConnector\\** by pressing **Next**.
   
   ![image](https://user-images.githubusercontent.com/112052485/224062686-471b422f-6dbb-415c-b540-0b17dffdaf4d.png)

   
   * Click **Next** to install
   * Click **Yes** to allow the installation when the **authentication** pops up
   * Once it finishes, click **Close**
   
8. Go to **Start -> All Programs -> Accessories -> Windows PowerShell**
9. Right click on **Windows PowerShell** and select **Run as Administrator**

   ![image](https://user-images.githubusercontent.com/112052485/224063563-f6ff6667-8f4d-4fa3-9a15-fac82ab9777e.png)


10. Click **Yes** to run with elevated privileges
11. Click **Yes** to allow the program to make changes to the computer
12. Type: ``Set-ExecutionPolicy Unrestricted`` at the Powershell prompt

   ![image](https://user-images.githubusercontent.com/112052485/224064847-4d96cb0f-6edf-4058-bb90-a6643051c408.png)


14. Press "Y" and enter



[Back to MS SQL Lab Guide](/README.md) | [Back to Workshop Guide](../README.md)
