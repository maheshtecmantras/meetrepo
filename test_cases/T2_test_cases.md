# Test Cases for T2 - Venues Management

Okay, I understand the task. Here are two detailed test cases for the "Venues Management" feature, targeting different aspects of the functionality.

**Test Case 1:  Venue Creation and Basic Information Validation**

*   **Title:** Verify Successful Venue Creation with Valid Basic Information

*   **Description:** This test case verifies that an administrator can successfully create a new venue using the Venues Management system, and that basic venue information (name, address, capacity) is correctly saved and displayed. This focuses on the fundamental functionality of adding a venue to the system.

*   **Steps:**

    1.  **Precondition:**  User is logged in as an administrator to the Venues Management system.
    2.  **Navigation:** Navigate to the "Venues Management" section (e.g., via a menu option or dashboard link).
    3.  **Action:** Click on the "Add New Venue" or equivalent button/link.
    4.  **Input:**  Enter the following information into the required fields:
        *   Venue Name: "The Grand Ballroom"
        *   Address Line 1: "123 Main Street"
        *   City: "Anytown"
        *   State/Province: "CA"
        *   Zip/Postal Code: "91234"
        *   Country: "USA"
        *   Capacity: "500"
    5.  **Input:**  Leave optional fields (e.g., Venue Description, Contact Phone Number, Website URL) blank.
    6.  **Action:** Click the "Save" or "Create Venue" button.
    7.  **Verification:** Observe the system's response after clicking "Save".

*   **Expected Result:**

    1.  The system displays a success message indicating the venue has been created successfully (e.g., "Venue 'The Grand Ballroom' created successfully.").
    2.  The user is redirected to the venue details page or a venue listing page.
    3.  On the venue details page or venue listing, the following information is accurately displayed:
        *   Venue Name: "The Grand Ballroom"
        *   Address: "123 Main Street, Anytown, CA 91234, USA" (formatted correctly)
        *   Capacity: "500"
    4.  The newly created venue is present in the venue listing, sorted according to the default sorting method (e.g., alphabetically by name or by creation date).
    5. The newly created venue's record can be found in the system database.

*   **Priority:** High (Core functionality)

**Test Case 2: Event Scheduling and Guestlist Management Validation**

*   **Title:** Verify Successful Event Scheduling and Guestlist Management

*   **Description:** This test case verifies that an administrator can successfully schedule an event at an existing venue through the Venues Management system, and that guest list functionalities work properly.

*   **Steps:**

    1.  **Precondition:**  User is logged in as an administrator to the Venues Management system. A venue "The Grand Ballroom" must exist (created from previous Test Case 1 or another method).
    2.  **Navigation:** Navigate to the "Venues Management" section (e.g., via a menu option or dashboard link).
    3.  **Action:** Find "The Grand Ballroom" venue from the venues management page and select the manage event section for the specific venue.
    4.  **Input:**  Enter the following information into the required fields:
        *   Event Name: "New Year's Eve Party"
        *   Event Date: "12/31/2024"
        *   Event Time: "9:00 PM"
    5.  **Action:** Click "Add" or "+" button in the Guest List section to add a new guest.
    6.  **Input:**  Enter the following information into the required fields for a guest:
        *   Guest Name: "John Doe"
        *   Email: "john.doe@example.com"
    7.  **Action:** Click "Save" or "Create Event" button.
    8.  **Verification:** Observe the system's response after clicking "Save".

*   **Expected Result:**

    1.  The system displays a success message indicating the event has been created successfully.
    2.  The user is redirected to the event details page or a event listing page.
    3.  On the event details page or event listing, the following information is accurately displayed:
        *   Event Name: "New Year's Eve Party"
        *   Event Date: "12/31/2024"
        *   Event Time: "9:00 PM"
    4.  The newly created event is present in the event listing, sorted according to the default sorting method (e.g., by name or by event date).
    5. On the event details page, the guest "John Doe" with the email "john.doe@example.com" should be listed.

*   **Priority:** High (Core functionality)

**Explanation of Choices:**

*   **Focus on Core Functionality:** These test cases target fundamental aspects of the Venues Management system: creating venues and scheduling events.
*   **Positive Testing:** They focus on "happy path" scenarios where valid data is entered.  Later test cases would cover negative scenarios (invalid data, missing fields, etc.).
*   **Clear Steps and Expected Results:**  The steps are detailed and unambiguous, allowing a tester to follow them easily.  The expected results are specific and measurable.
*   **Priority:**  Both test cases are marked as "High" priority because they are essential for the basic functionality of the Venues Management feature to work correctly.

These are just two example test cases. A complete test plan would include many more test cases covering various scenarios, edge cases, and error handling.