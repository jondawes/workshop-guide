## <a id="exercise11">Exercise 11 - Set a New Retention Policy

There are four types of Policies in Delphix. In this exercise, you will:

  * Create a Retention Policy

  * Set the new policy to keep snapshots and logs for 30 days, along with 3 monthly snapshots

  * Apply the policy to the VDB we created in the previous exercise

Both dSources and VDBs timeflow is governed by snapshots, which are either created manually or through policies. Retention policies govern the lifespan of such snapshots and help clean older ones that are no longer relevant.

**Steps**

  1. Navigate to Manage -> Policies

  2. Create a new retention policy (by going to the "Retention" tab and clicking the "+ Retention" blue button) for _devdb_ with the following details:

    1. Name: Long Term

    2. 30 days of snapshot and log retention

    3. 3 monthly snapshots taken on the 1st of the month

  3. To do this click on **+ Retention** and then fill the fields as shown in the screenshot below:

![images/download/attachments/90015915/worddav892f27227ee91e11f31c2a77d0808e3d.png](images/download/attachments/90015915/worddav892f27227ee91e11f31c2a77d0808e3d.png)

  1. Click Next and select **devdb** on the bottom of the pop up and then click Submit.

  [Back to MS SQL Lab Guide](/README.md) | [Back to Workshop Guide](../README.md)