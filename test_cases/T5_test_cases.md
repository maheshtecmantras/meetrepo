# Test Cases for T5 - Users Management

Okay, here are two detailed test cases based on the provided "Users Management" task description. I've focused on different areas of the functionality to provide broader coverage.

**Test Case 1: User Invitation and Activation**

*   **Title:** Verify Successful User Invitation and Account Activation

*   **Description:** This test case verifies the functionality of inviting a new user to the PuraVida platform, ensuring the invitation is sent correctly, the user receives the invitation, and is able to successfully activate their account.

*   **Steps:**

    1.  **Pre-condition:** An administrator user is logged into the PuraVida platform with appropriate user management permissions.
    2.  Navigate to the "Users Management" section.
    3.  Click on the "Invite User" or similar button/link.
    4.  Enter a valid, unused email address in the "Email Address" field.  (e.g., `test.user.invite.123@example.com`)
    5.  If required, fill in the user's first name, last name, and any other mandatory fields (e.g., role, group). For the sake of this test, use valid data. "First Name": TestUser, "Last Name": Invitation
    6.  Click the "Send Invitation" or similar button/link.
    7.  Check that a confirmation message is displayed on the screen (e.g., "Invitation sent successfully").
    8.  **Verification Step (External - Email System):** Access the email inbox of the email address used in Step 4. (This may require access to a test email server/account or a configured email testing framework).
    9.  Verify that an invitation email from PuraVida has been received.
    10. Verify that the invitation email contains:
        *   The name of the PuraVida platform.
        *   A clear and concise message explaining the invitation.
        *   A unique activation link.
    11. Click the activation link in the invitation email.
    12. The user should be redirected to the PuraVida platform to a registration/activation page.
    13. Fill in the required fields on the activation page (e.g., create a password, confirm password, agree to terms). Use a strong and valid password.
    14. Click the "Activate Account" or similar button/link.

*   **Expected Result:**

    1.  A confirmation message indicating successful invitation is displayed in the UI.
    2.  An invitation email is successfully sent to the specified email address.
    3.  The invitation email contains the correct information, including a unique and valid activation link.
    4.  Clicking the activation link redirects the user to the activation page.
    5.  The user is able to successfully create an account by filling in the required information and clicking the "Activate Account" button.
    6.  After clicking the "Activate Account" button, the user is successfully logged into the PuraVida platform (or redirected to the login page with a success message).

*   **Priority:** High (Core functionality; prevents new users from joining the platform)

<br/>

**Test Case 2: User Profile Viewing and Status**

*   **Title:** Verify Ability to View User Profiles and Their Status.

*   **Description:** This test case verifies that an administrator can successfully view the profile details of existing users and check their current status within the PuraVida platform.

*   **Steps:**

    1.  **Pre-condition:** An administrator user is logged into the PuraVida platform with appropriate user management permissions. At least one user account (other than the administrator) exists on the platform with a known status (e.g., Active, Inactive, Pending).
    2.  Navigate to the "Users Management" section.
    3.  Locate the user list or table.
    4.  Search for the user account (created in pre-condition step) either by using the search functionality or by browsing the user list.
    5.  Click on the user's name or a "View Profile" button/link associated with the user.
    6.  Verify that the user's profile details are displayed, including:
        *   User's Full Name
        *   Email Address
        *   User Status (Active, Inactive, Pending, etc.)
        *   Role or Permissions
        *   Join Date
        *   Last Login Date (if available)
        *   Membership Details (if relevant)
        *   Referral Information (if relevant) - Referrer and Referee details.
    7.  Verify that all displayed profile information matches the actual data associated with the user in the system's database.
    8.  Repeat steps 4-7 for users with different statuses (e.g., Active, Inactive, Pending) to ensure the status is accurately displayed.

*   **Expected Result:**

    1.  The administrator is able to successfully navigate to the user list/table.
    2.  The administrator can locate the desired user account using search or browsing.
    3.  Clicking on the user's name or "View Profile" link displays the user's profile details.
    4.  All relevant user profile details are displayed accurately, including Name, Email, Status, Role, Dates, and any relevant membership or referral data.
    5.  The displayed user status correctly reflects the actual status of the user in the system.

*   **Priority:** High (Essential for user management and monitoring user activity)