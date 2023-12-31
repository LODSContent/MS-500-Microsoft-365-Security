---
lab:
    title: 'Lab2: Exercise 4 - Directory Roles (General) '
    type: 'Answer Key'
    module: 'Module 3: Identity and Access Management'
---

# Module 3 - Lab 2 - Exercise 4 - Directory Roles (General)


### Task 1: Start an access review for Azure AD directory roles in PIM


Role assignments become "stale" when users have privileged access that they don't need anymore. In order to reduce the risk associated with these stale role assignments, privileged role administrators or global administrators should regularly create access reviews to ask admins to review the roles that users have been given. This task covers the steps for starting an access review in Azure AD Privileged Identity Management (PIM).


1.  Return back to the browser that is logged in to the Azure portal as your Global Admin Account Holly Dickson.

1.  From the PIM application main page select **Azure AD Roles** > **Access reviews** > **New**.

1.  Enter the following details and click **Start**:

      - Review name:  `Global Admin Review`
      - Start Date:  `Enter Today's Date` 
      - Frequency: `Drop down to One time`
      - End Date:  `Enter End of next month`
      - Role:  `Global Administrator`
      - Reviewers:  `Holly Dickson`
 
1.  Once the review has completed and has a status of Active, click on the **Global Admin Review**. You may need to refresh the view in Azure.

1.  Select **Results** and see the outcome of **Not reviewed** in the **Outcome** column for each of the results.

### Task 2: Approve or deny access


When you approve or deny access, you are just telling the reviewer whether you still use this role or not. Choose Approve if you want to stay in the role, or Deny if you don't need the access anymore. Your status won't change right away, until the reviewer applies the results. Follow these steps to find and complete the access review:


1.  In the PIM application, select **Review access**. 

2.  Select the **Global Admin Review**.

     ![Screenshot](../Media/3f5a8e6a-05a7-4cc0-96ea-d1a10d23c38f.png)

3.  You can **View** the audit details for any of the role memberships which you would like to investigate.

5.  Close the **Global Admin Review** and **Review Azure AD roles** blade.

### Task 3: Complete an access review for Azure AD directory roles in PIM


Privileged role administrators can review privileged access once an access review has been started. Azure AD Privileged Identity Management (PIM) will automatically send an email prompting users to review their access. If a user did not get an email, you can send them the instructions in how to perform an access review.

After the access review period is over, or all the users have finished their self-review, follow the steps in this task  to manage the review and see the results.



1. Return to the `Global Admin Review`. Go to the **Azure portal** > `Azure AD Privileged Identity Management` > **Azure AD Roles** > **Access reviews** > `Global Admin Review`. 

4. Choose one of the available options for completing the review:
     - **Stop** - All access reviews have an end date, but you can use the Stop button to finish it early. If any users haven't been reviewed by this time, they won't be able to after you stop the review. You cannot restart a review after it's been stopped.
     - **Apply** - After an access review is completed, either because you reached the end date or stopped it manually, the Apply button implements the outcome of the review. If a user's access was denied in the review, this is the step that will remove their role assignment.
     - **Delete** - If you are not interested in the review any further, delete it. The Delete button removes the review from the Privileged Identity Management service.


### Task 4: Configure security alerts for Azure AD directory roles in PIM

You can customize some of the security alerts in PIM to work with your environment and security goals. Follow these steps to open the security alert settings:

1. Open `Azure AD Privileged Identity Management` > **Azure AD roles** > **Alerts** > **Setting**.
1. Click an alert name to configure the setting for that alert.

# continue to exercise 5
