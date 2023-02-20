## <a id="exercise5"></a>Exercise 5 - Create a Target Environment

In this exercise, you will:

  * Connect Delphix to your Windows Target server

The target environment is the host where the virtual databases will be created.

## Steps
1. Navigate to your Delphix Engine at 10.0.x.10 ('x' is your **Student Number** )
  * Log in as the delphix_admin user
  * Go to Manage -> Environments
  * Click the ellipses (…) and select _Add Environment_
  
![images/download/attachments/90015915/worddava57004a26ec15405b106bc030428200a.png](images/download/attachments/90015915/worddava57004a26ec15405b106bc030428200a.png)

2. On the _Host and Server_ tab choose **Windows** as the _Host OS_ and **Target** as the _Host Type_ then click Next

  ![images/download/attachments/90015915/worddav8207f96e2ec2346bb3593fca6d19d381.png](images/download/attachments/90015915/worddav8207f96e2ec2346bb3593fca6d19d381.png)
  
3. Under the Environment Settings tab, enter the details:
  * Environment Name: WINTARGET
  * Host Address: 10.0.x.60 (`x` is your **Student Number** )
  * Delphix Connector port: 9100
  * OS Username: delphix\delphix_trgt
  * OS Password: delphix
  * Click Validate Credentials
  * Click Submit
The creation is successful when "Create and discover environment 10.0.x.60"
completes without error and WINTARGET appears on your Delphix Environments
page

  ![images/download/attachments/90015915/worddavb5ed0882a1929025813b0acc1a617a87.png](images/download/attachments/90015915/worddavb5ed0882a1929025813b0acc1a617a87.png)

  [Back to MS SQL Lab Guide](/README.md) | [Back to Workshop Guide](../README.md)