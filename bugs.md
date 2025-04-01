# Linq QA Assessment - Bugs

## 1. 'Exchange Contact'text updated to 'Contact Saved' incorrectly  
**Description:** Clicking the 'Exchange Contact' button but not actually downloading or saving the contact still results in the 'Contact Saved' text. The user did not save any info, but the UI incorrectly reflects that the action was completed.  
**Steps to Reproduce:**  
1. Load a public Linq profile.  
2. Click on the "Exchange Contact" button.  
3. Do not download the contact or enter any information.  
4. Validate that the "Exchange Contact" button updates to "Contact Saved" without actually saving the contact info.  
**Expected Result:** The button should remain as "Exchange Contact" unless the user successfully saves or exchanges contact information.  
**Actual Result:** The button updates to "Contact Saved" even when no contact is downloaded or exchanged.  

[Exchange Contact Text Updated to Contact Saved Incorrectly](./images/bugs/Recording%202025-04-01%20093214.mp4)

---

## 2. Exchange Info Popup Not Closing After Save  
**Description:** After the user successfully saves a contact, the 'Exchange Info' pop-up remains displayed, preventing the success message from being visible.  
**Steps to Reproduce:**  
1. Load a public Linq profile.  
2. Click on the "Exchange Contact" button.  
3. Download the contact or enter information and click continue.  
4. Validate that the 'Exchange Info' pop-up does not close, blocking the success message.  
**Expected Result:** The pop-up should automatically close after successful contact save, allowing the success message to be visible.  
**Actual Result:** The pop-up remains open, covering the success confirmation.  

![Exchange info pop-up not closing after save](./images/bugs/Screenshot%202025-04-01%20091923.png)


