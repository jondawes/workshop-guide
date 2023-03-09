## <a id="exercise6"></a>Exercise 6 - Add the Source Environment

In this exercise, you will:

  * Connect Delphix to your Windows Source Server

Before users can create their own virtual databases, Delphix needs to connect to source data. In Delphix, an environment is a host that runs database software. The environment is where the Delphix engine will search for available data sources. Credentials to access the host need to be provided while configuring an environment.

### Steps

1. Navigate to your **Delphix Engine** at 10.0.x.10 ('x' is your **Student Number** )
2. Log in as the _**admin**_ user
3. Go to **Manage -> Environments**
4. Click the ellipses (…) after **Environments** on the left-hand side of the screen and click on **Add Environment**
5. Click **Windows Source** and **Standalone**
6. Enter the details:
   a. Environment Name: _**WINSOURCE**_
   b. Host Address: **10.0.x.50** (‘x’ is your **Student Number**)
   c. Connector Environment: Click on **WINTARGET**
   d. OS Username: _**delphix\delphix_src**_
   e. OS Password: _**delphix**_
7. Click **Validate**
8. Click **Next**

![image](https://user-images.githubusercontent.com/112052485/224073184-23cc2c69-c65e-46f3-ae99-377db3dc9c1b.png)


9. Click **Submit**


The creation is successful when "Create and discover environment 10.0.x.50"
completes without error and WINSOURCE appears on your Delphix Environments
page.

![image](https://user-images.githubusercontent.com/112052485/224073492-9b93c6d6-2a69-4afa-b010-50db56cd6281.png)


[Back to MS SQL Lab Guide](/README.md) | [Back to Workshop Guide](../README.md)
