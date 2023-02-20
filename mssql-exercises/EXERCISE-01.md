## <a id="exercise1"></a>Exercise 1 - Delphix Engine Configuration

In this exercise, you will:
  * Access the Delphix Engine GUI for the first time
  * Set up the Delphix SYSADMIN user
  * Configure Timezone Preferences
  * Configure Network Settings
  * Configure Disks
  * Complete the Delphix Engine configuration
  * Set up the DELPHIX_ADMIN user

### Steps

1. Connect to your Delphix Engine using Chrome on your lab server (see the **Important IP Addresses** section of the Getting Started guide above).
2. Set the new sysadmin password to: delphix
3. Configure the Delphix Engine with the following details:
  * NTP on using pool.ntp.org with your local timezone
  * Default network settings
  * Three 8GB volumes in the data pool
  * Default Serviceability options
  * Default Authentication Service options
  * Appliance marked registered (no support credentials are required for this lab)
  * Completed and saved System setup.
4. Log in with the _admin_ user (password = 'delphix')
5. When prompted, set the new _admin_ password to: delphix

You will know this is successful when you see the main Delphix UI screen with
a single group (Untitled) on the left hand side.

 **Related Links**
[The delphix_admin and sysadmin User
Roles](https://docs.delphix.com/display/DOCS43/The+delphix_admin+and+sysadmin+User+Roles)
[Setting Up the Delphix
Engine](https://docs.delphix.com/display/DOCS43/Setting+Up+the+Delphix+Engine)

[Back to MS SQL Lab Guide](/README.md) | [Back to Workshop Guide](../README.md)