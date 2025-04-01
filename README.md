# Linq QA Assessment  

This repo has my QA assessment, covering manual testing, bugs found, API testing and a bonus markdown.  

## Files
- **test-cases.md** – A list of manual test cases for verifying the Linq profile and contact-saving functionality.  
- **bugs.md** – Issues found during testing, with steps to reproduce, expected vs. actual behavior, and screenshots.  
- **postman-notes.md** – API testing using Postman, with key takeaways.
- **bonus.md** – Suggestions that stick out from my exploratory testing.  

## Bug Findings  
- Contact saving does not validate if the user successfully downloads the contact before marking it as "Contact Saved."  
- No authentication required to download contacts, which may pose a security risk.  
- The ‘Exchange Info’ pop-up does not close after saving a contact, blocking the success message.  

