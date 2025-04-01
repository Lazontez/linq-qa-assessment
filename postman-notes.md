# Postman Notes
---

## **API**
### **Steps Taken:**
1. Used Postman to simulate saving a contact by making API requests to Linq.
2. Captured request headers, payloads, and responses.
3. Used browser dev tools to cross-check network activity during contact-save.

---

## **API Request Details**
### **Request URL:**
`https://api.linqapp.com/api/v1/cards/football_fred/download_contact`

### **Method:**
`GET`

### **Headers Sent:**

`accept: application/json content-type: application/json origin: https://linqapp.com referer: https://linqapp.com/ x-linq-api-token: null user-agent: Mozilla/5.0 (Linux; Android 8.0.0; SM-G955U Build/R16NW) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/134.0.0.0 Mobile Safari/537.36 Edg/134.0.0.0`


### **Response Details:**
- **Status:** `200 OK`
- **File Received:** `Football_Fred2261111.vcf`
---

## **Findings**

###  **Contact Saving Behavior**
- The request successfully retrieves a `.vcf` file, allowing the contact to be downloaded.
- Note: There is no validation step to confirm if the contact was actually saved on the device.

###  **Concerns**
#### **No Authentication Required**
- The API token is `null`, but the request still retrieves the vCard.
- This means anyone with the URL format has the ability to access and download contacts, which could be a data exposure risk if private contacts are involved.

#### **CORS & Access Control**
- `access-control-allow-origin: https://linqapp.com` ensures only Linq’s domain can request the resource, but more validation should be confirmed to prevent unauthorized access.

### **Headers & Caching Behavior**
- `cache-control: private` prevents the response from being cached publicly.
- `etag` and `if-none-match` suggest caching, duplicate requests may not trigger new API responses, could affect real-time changes.

---


