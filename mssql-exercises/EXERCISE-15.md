## <a id="exercise15">Exercise 15 - Delink a dSource

In this exercise you will

  * Delink a dSource

  * Note the changes to Timeline of the dSource caused by the delink operation

  * Note the VDB provisioned from the delinked dSource is unaffected.

Steps

1. Login to the Delphix Admin UI as a user with Delphix_Admin privileges.

2. Navigate to Manage  Datasets and click on the dSource "Adventureworks2008R2"

3. Unlink the dSource - Click on the ellipses (…) next to snapshot button and click on "Unlink dSource"

![images/download/attachments/90015915/worddav6ba203cca87a2644f98038d04e80ed11.png](images/download/attachments/90015915/worddav6ba203cca87a2644f98038d04e80ed11.png)

4. Click Unlink on the confirmation box that pops up.

5. Once action completes note the status of the dSource on the right hand side has changed to Detached. You will be unable to take additional snapshots of a detached dSource.

6. Note changes in the display. Click on Status and Configuration tabs and notice the changes.

7. Connect to the target VDB and confirm it is still running.

[Back to MS SQL Lab Guide](/README.md) | [Back to Workshop Guide](../README.md)