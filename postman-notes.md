# Linq QA Assessment Test Cases

### 1.
**Test Case ID:** TC001  
**Description:** Validate that a visitor can view a public profile on a desktop browser and that all elements are displayed correctly.  
**Preconditions:** The user has access to a valid Linq profile URL.  
**Test Steps:**  
1. **Load a Linq profile from a desktop browser (Chrome, Firefox, or Safari).**  
   - **Expected Result:** The Linq profile successfully loads without any errors.  
2. **Validate all profile details (name, contact info, links, profile image) are displayed correctly.**  
   - **Expected Result:** All data related to the profile should be displayed as expected.  
3. **Validated that no UI elements overlap or are cut off.**  
   - **Expected Result:** UI elements should match the expected design document.

---

### 2.
**Test Case ID:** TC002  
**Description:** Validate that a user can view a public profile on a mobile browser with a responsive layout.  
**Preconditions:** The user has access to a valid Linq profile URL.  
**Test Steps:**  
1. **Load a Linq profile from a mobile browser (Chrome, Firefox, or Safari).**  
   - **Expected Result:** The Linq profile should load successfully without issue.  
2. **Validate all profile details associated with the account (e.g., name, contact info, links, profile image) are displayed correctly.**  
   - **Expected Result:** All data related to the profile account should be displayed without error.  
3. **Validate that the page is optimized for mobile screens.**  
   - **Expected Result:** The profile loads fully with correct details in a mobile-friendly layout and matches the design document for mobile view.

---

### 3.
**Test Case ID:** TC003  
**Description:** Validate that a user can save a contact on a desktop device and receive appropriate feedback.  
**Preconditions:** The user has access to a public Linq profile.  
**Test Steps:**  
1. **Load a public Linq profile on a desktop browser.**  
   - **Expected Result:** The profile should successfully load without issue.  
2. **Click on the "Exchange Contact" button.**  
   - **Expected Result:** The 'Exchange Info' pop-up is displayed.  
3. **Validate that the correct fields and buttons are displayed in the 'Exchange Contact' pop-up (Name, Phone, Email, Continue button, and Download Contact link).**  
   - **Expected Result:** All required fields, buttons and links are displayed as expected.  
4. **Click the 'Download Contact' link.**  
   - **Expected Result:** A success message appears confirming that the contact was saved and the 'Exchange Info' pop=up us no longer displayed.  
5. **Validate the 'Share your info' input fields and enter valid information.**  
   - **Expected Result:** The user should successfully enter and send their info to the Linq profile account.  
6. **Validate that the "Exchange Contact" button is updated to "Contact Saved".**  
   - **Expected Result:** Once the user has saved the profile’s contact information, the button updates to "Contact Saved".

---

### 4.
**Test Case ID:** TC004  
**Description:** Validate that a visitor can save a contact on a mobile device.  
**Preconditions:** The user has access to a valid Linq profile URL on a mobile device.  
**Test Steps:**  
1. **Load a public Linq profile on a mobile browser (Chrome, Firefox, or Safari on iOS/Android).**  
   - **Expected Result:** The profile should successfully load without issue.  
2. **Click the "Exchange Contact" button.**  
   - **Expected Result:** The 'Exchange Info' pop-up is displayed.  
3. **Validate the correct fields and buttons are displayed in the 'Exchange Contact' pop-up (Name, Phone, Email, Continue button, and Download Contact link).**  
   - **Expected Result:** All required elements are displayed as expected.  
4. **Click the 'Download Contact' link.**  
   - **Expected Result:** A success message appears confirming that the contact was saved and Exchange Info pop-up should no longer be displayed.  
5. **Validate the 'Share your info' input fields and enter valid information.**  
   - **Expected Result:** The user should successfully enter and send their info to the Linq profile account.  
6. **Validate that the "Exchange Contact" button is updated to "Contact Saved".**  
   - **Expected Result:** The button updates to "Contact Saved", indicating the contact has been saved.

---

### 5.
**Test Case ID:** TC005  
**Description:** Validate that a visitor can save a contact on a device even if it has been saved before..  
**Preconditions:** The user previously saved the contact on the same device.  
**Test Steps:**  
1. **Load a public Linq profile on a device where the contact has been previously saved.**  
   - **Expected Result:** The profile should successfully load without issue.  
2. **Click on the "Exchange Contact" button.**  
   - **Expected Result:** The 'Exchange Info' pop-up is displayed.  
3. **Click the 'Download Contact' link to save the contact again.**  
   - **Expected Result:** The system allows the contact to be saved again.  
4. **Validate that the system handles the duplicated save correctly (Example: by updating the existing contact's details or indicating a re-save action, maybe adding any new details from the profile to account).**  
   - **Expected Result:** The contact is saved without creating an unintended duplicate entry, and the user receives confirmation and appropriate feedback.

---

### 6.
**Test Case ID:** TC006  
**Description:** Validate that the Linq profile page is accessible via a screen reader.  
**Preconditions:** The user has a screen reader enabled (e.g., NVDA, JAWS, or VoiceOver) and access to  valid Linq profile.
**Test Steps:**  
1. **Load a public Linq profile with the screen reader enabled.**  
   - **Expected Result:** The profile should successfully load without issue.  
2. **Navigate through the profile using keyboard controls and the screen reader.**  
   - **Expected Result:** All profile details (name, contact info, links, profile image) should be read correctly.  
3. **Attempt to activate the "Exchange Contact" button using keyboard navigation.**  
   - **Expected Result:** The button should be accessible and properly announced by the screen reader.  
4. **Follow the process for saving a contact using the screen reader.**  
   - **Expected Result:** Each step should be clearly announced and navigable, ensuring full accessibility compliance.

---

### 7.
**Test Case ID:** TC007  
**Description:** Validate that the system handles API failures when saving a contact.  
**Preconditions:** The user has access to a valid Linq profile URL and the ability to do mock network/API issues.  
**Test Steps:**  
1. **Load a public Linq profile.**  
   - **Expected Result:** The profile should successfully load without issue.  
2. **Click on the "Exchange Contact" button.**  
   - **Expected Result:** The 'Exchange Info' pop-up is displayed.  
3. **Simulate an API failure (Example: disable network connectivity or use tool to send a bad request).**  
   - **Expected Result:** The system should attempt to process the request despite the failure.  
4. **Observe the system’s response.**  
   - **Expected Result:** A clear error message should be displayed, informing the user of the API failure, and the process should handle the error gracefully.

---


### 8.
**Test Case ID:** TC009  
**Description:** Validate that saving a contact works consistently across different web browsers.  
**Preconditions:** The user has access to a valid Linq profile URL on multiple browsers.  
**Test Steps:**  
1. **Load a public Linq profile on Google Chrome.**  
   - **Expected Result:** The profile should successfully load without issue.  
2. **Click on the "Exchange Contact" button.**  
   - **Expected Result:** The 'Exchange Info' pop-up is displayed and functions correctly.  
3. **Repeat steps 1 and 2 on Mozilla Firefox and Safari (both desktop and mobile if applicable).**  
   - **Expected Result:** The profile loads and the exchange contact process works consistently across all tested browsers.  
4. **Compare the results across browsers.**  
   - **Expected Result:** The process should eb consistent, with no browser-specific UI/UX discrepancies.
