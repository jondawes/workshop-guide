## <a id="exercise6"></a>Exercise 6 - Add the Source Environment

In this exercise, you will:

  * Connect Delphix to your Windows Source Server

Before users can create their own virtual databases, Delphix needs to connect to source data. In Delphix, an environment is a host that runs database software. The environment is where the Delphix engine will search for available data sources. Credentials to access the host need to be provided while configuring an environment.

### Steps

1. Navigate to your Delphix Engine at 10.0.x.10 ('x' is your **Student Number** )
2. Log in as the delphix_admin user
3. Go to Manage -> Environments
4. Click the ellipses (…) and select _Add Environment_
5. On the _Host and Server_ tab choose **Windows** as the _Host OS,_ **Source** as the _Host Type_ and **Standalone** as the _Server Type_ then click Next
6. Enter the details:
  * Environment Name: WINSOURCE
  * Host Address: 10.0.x.50 ('x' is your **Student Number** )
  * Connector Environment: Click on WINTARGET
  * OS Username: delphix\delphix_src
  * OS Password: delphix
7. Click Validate Credentials
8. Click Submit

  ![images/download/attachments/90015915/worddave7d4c3b1ae491d7bf599dd31fc8b7dce.png](images/download/attachments/90015915/worddave7d4c3b1ae491d7bf599dd31fc8b7dce.png)

The creation is successful when "Create and discover environment 10.0.x.50"
completes without error and WINSOURCE appears on your Delphix Environments
page

[Back to MS SQL Lab Guide](/README.md) | [Back to Workshop Guide](../README.md)