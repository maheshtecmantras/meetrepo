# Test Cases for T1 - Dashboard

Okay, here are two detailed test cases for the Dashboard, based on the provided task. I've focused on two different, but essential, aspects of the Dashboard: data accuracy and visual presentation/responsiveness.

**Test Case 1: Data Accuracy on Admin Dashboard**

*   **Title:** Verify Accuracy of Key Metrics on Admin Dashboard

*   **Description:** This test case verifies the accuracy of the key metrics displayed on the Admin Dashboard by comparing the reported values to the data stored in the back-end database. This ensures that the dashboard provides reliable and actionable insights for administrators.

*   **Steps:**

    1.  **Pre-Condition:** Log in as an administrator with full access privileges.
    2.  **Navigation:** Navigate to the Admin Dashboard.
    3.  **Data Extraction (Database):** Access the back-end database (e.g., using SQL queries or a suitable database administration tool). Extract the following data points for the relevant reporting period (e.g., current day, week, month, as specified on the dashboard):
        *   Total number of registered users.
        *   Total number of active users (defined as users logged in at least once within the reporting period).
        *   Total number of venues.
        *   Total number of approved venues.
        *   Total number of pending venue approval requests.
        *   Total number of completed bookings (if booking data is displayed).
        *   Total revenue generated (if revenue data is displayed).
    4.  **Data Extraction (Dashboard):**  Manually record the values displayed on the Admin Dashboard for each of the corresponding metrics extracted in Step 3.
    5.  **Data Comparison:** Compare the values extracted from the database in Step 3 with the values displayed on the Dashboard in Step 4.  Consider any specified refresh intervals for the dashboard data. Note any discrepancies.

*   **Expected Result:**

    *   All metrics displayed on the Admin Dashboard should match the corresponding values retrieved directly from the back-end database within a reasonable margin of error (e.g., +/- 1%, or a defined threshold for specific metrics where slight discrepancies are expected due to real-time updates).
    *   If refresh intervals are specified, the dashboard should update within the defined timeframe.
    *   Any discrepancies must be investigated and resolved.

*   **Priority:** High

**Test Case 2: Dashboard Responsiveness and Visual Presentation**

*   **Title:** Verify Responsive Layout and Visual Presentation of Admin Dashboard Across Various Devices and Browsers.

*   **Description:** This test case verifies that the Admin Dashboard displays correctly and remains functional across different screen sizes, devices (desktop, tablet, mobile), and browsers. It also covers UI elements (alignment, fonts, colors) are displayed as designed.

*   **Steps:**

    1.  **Pre-Condition:** Log in as an administrator with full access privileges.
    2.  **Navigation:** Navigate to the Admin Dashboard.
    3.  **Device/Browser Selection:** Select the following devices/browsers for testing (this list should be expanded to cover all supported platforms):
        *   Desktop: Chrome, Firefox, Safari, Edge (at various screen resolutions).
        *   Tablet (Landscape and Portrait): iPad, Android Tablet (at various screen resolutions).
        *   Mobile (Landscape and Portrait): iPhone, Android Phone (at various screen resolutions).
    4.  **Verification (Desktop):**
        *   **Resizing:** Resize the browser window to different widths and heights.  Observe that the dashboard elements reflow and adjust appropriately.
        *   **Scrollbars:** Verify that scrollbars appear only when necessary (i.e., when the content exceeds the visible area).
        *   **Alignment:** Ensure that all elements (text, images, charts, buttons) are properly aligned and spaced, without overlapping or truncation.
        *   **Font and Colors:** Verify that the fonts and colors used are consistent with the design specifications and are easily readable.
        *   **Clickable Elements:** Ensure that all clickable elements (buttons, links, chart elements) are easily clickable and responsive.
    5.  **Verification (Tablet and Mobile):**
        *   **Orientation Changes:** Rotate the device between portrait and landscape orientations. Observe that the dashboard layout adapts correctly.
        *   **Touch Gestures:** Verify that touch gestures (scrolling, zooming, tapping) work as expected.
        *   **Responsiveness:** Ensure that the dashboard elements are appropriately sized and spaced for the smaller screen sizes.
        *   **Element Visibility:** Verify that all critical dashboard elements are visible and accessible without excessive scrolling.
    6.  **Browser-Specific Issues:** Pay attention to any browser-specific rendering issues (e.g., font rendering differences, CSS compatibility problems).

*   **Expected Result:**

    *   The Admin Dashboard should display correctly and be fully functional across all supported devices and browsers.
    *   The dashboard layout should be responsive, adapting to different screen sizes and orientations without breaking.
    *   All elements (text, images, charts, buttons) should be properly aligned, spaced, and readable.
    *   Touch gestures should work as expected on touch-enabled devices.
    *   There should be no browser-specific rendering issues that significantly degrade the user experience.

*   **Priority:** High