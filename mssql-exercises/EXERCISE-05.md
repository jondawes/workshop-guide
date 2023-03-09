## <a id="exercise5"></a>Exercise 5 - Create a Target Environment

In this exercise, you will:

  * Connect Delphix to your Windows Target server

The target environment is the host where the virtual databases will be created.

## Steps
1. Navigate to your **Delphix Engine** at 10.0.x.10 ('x' is your **Student Number** )
2. Log in as the _**admin**_ user
3. Go to **Manage -> Environments**
4. Click the ellipses (…) after **Environments** on the left hand side of the screen and click on **Add Environment**
5. Click **Windows**, **Target** and **Standalone**
6. Click **Next**
7. Under the **Environment Settings** tab section, enter the details:
   a. Environment Name: **WINTARGET**
   b. Host Address: **10.0.x.60** (`x` is your Student Number)
   c. Delphix Connector port: **9100**
   d. Skip **DSP** entries
   e. OS Username: **_delphix\delphix_trgt_**
   f. OS Password: **_delphix_**
8. Click **Validate**
  
![image](https://user-images.githubusercontent.com/112052485/224069767-ba6c9946-65c2-4256-9b4d-f4d638462e3a.png)


9. Click **Next**
10. Review the **Add Environment Summary**
11. Click **Submit**

The creation is successful when **Create and discover environment 10.0.x.60** completes without error and **WINTARGET** appears on your **Delphix Environments** page. 



  [Back to MS SQL Lab Guide](/README.md) | [Back to Workshop Guide](../README.md)
