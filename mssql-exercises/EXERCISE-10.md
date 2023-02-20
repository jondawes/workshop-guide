## <a id="exercise10">Exercise10 - Rewind a VDB

In this exercise, you will:

  * Take a snapshot of the _devdb_ VDB

  * Delete a table

  * Rewind the _devdb_ VDB to recover the table

Rewinding a VDB rolls it back to a previous point in its Timeflow and re-provisions the VDB. The VDB will no longer contain changes after the rewind point. it can be triggered when changes to the VDB do not need to be saved.

**Steps**

  1. Take a snapshot of the _devdb_ VDB and note the time

![images/download/attachments/90015915/worddav85bed0f1f0f83ce8d92d2dd8f66dff40.png](images/download/attachments/90015915/worddav85bed0f1f0f83ce8d92d2dd8f66dff40.png)

  1. Log into the Target via RDP

  2. Go to Start -> All Programs -> Microsoft SQL Server 2008 R2 -> SQL Server Management Studio

    1. Under Authentication, select "SQL Server Authentication"

    2. Log in as sa/delphix

  3. Expand "Databases"

  4. Right click **devdb** , then select New Query

  5. Run the following commands:

_drop table sourcetab;_
 _select count(*) from sourcetab;_

You will receive an error "Invalid Object name 'sourctab'.
Do not close the query window.
Now we will rewind the VDB to the last good snapshot to recover the table.

  1. Select the _devdb_ VDB

  2. Select the snapshot card associated with the date/time you recorded prior to dropping the table.

  3. Rewind the VDB to the snapshot card.

Once the rewind operation is complete, you can confirm the table has been
recovered:
Go to SQL Server Management Studio on Target SQL server and run the following
command.
 _select
count(*) from sourcetab;_
The should receive a count of the table.

[Back to MS SQL Lab Guide](/README.md) | [Back to Workshop Guide](../README.md)