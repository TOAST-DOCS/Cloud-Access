# User

**Security > Cloud Access > Console User Guide > User**

In the **User** tab, you can manage the policies for user accounts that connect after installing the agent.

<br>

## Manage User Accounts

### Add

Click **Add** to add a user account.

![user_add_1.PNG](https://kr1-api-object-storage.nhncloudservice.com/v1/AUTH_2acdfabf4efe4efc8a04c00b348110c9/cdn_origin/prod_cloud_access/2025.06.24/user_add_1.png)

* ➊ Basic Settings: Enter basic information for the user who will use the account, such as account name, mobile phone number, and email. 
* ➋ Account Settings: Configure the policy to be applied to the account.
    * Account Status: Set the account to allow or block after adding the user.
    * Private IP Address: When the user logs in, an IP is automatically assigned according to the user policy.
    * User Policy: Select the policy to apply to the user. Pre-registered policies are shown in the **Policy - User Policy** tab. 
    * Account Usage Time: You can restrict the available time within 24 hours (e.g., 9:00 AM–6:00 PM).
    * Account Validity Period: Set the duration the account can be used.
    * Inactive Account Lock: If the account is not used for a certain period, it will be automatically locked.
    * Allowed IP/MAC Addresses: You can specify up to three IP or MAC addresses that can log in using the account.

### Modify

Click **Modify** to modify the user account.

### Delete

Click **Delete** to delete the user account.

### Additional Features

* Download Template: Download the template file required for bulk registration.
* Upload User in Batch: Register multiple users at once using the downloaded template file.

![user_add_2.PNG](https://kr1-api-object-storage.nhncloudservice.com/v1/AUTH_2acdfabf4efe4efc8a04c00b348110c9/cdn_origin/prod_cloud_access/2025.06.24/user_add_2.png)

➊: File Upload: Click the file selection button to upload a file.
➋: Display Error Data: After verifying the uploaded file, displays any data with errors.

* Download User in Batch: Download the full list of users created in the **User** tab at once.

<br>

!!! danger "Caution"
    * The information required for authentication will be sent to the phone number and email address you provide, so please make sure to enter them correctly.