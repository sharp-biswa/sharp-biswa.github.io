# 📊 Google Sheets as a Database for Your Portfolio

Turn a free private Google Sheet into a live query database for your portfolio contact form in **under 2 minutes**.

Whenever a visitor submits the contact form, a new row is automatically added to your Google Sheet with their **Timestamp, Full Name, Email, and Message**.

---

## ⚡ Step-by-Step Setup Guide

### Step 1: Create a Google Sheet
1. Go to [sheets.new](https://sheets.new) (creates a new Google Sheet).
2. Name the sheet: **`Portfolio Inquiries`**.
3. (Optional) In row 1, set the column headers:
   - **A1:** `Timestamp`
   - **B1:** `Full Name`
   - **C1:** `Email`
   - **D1:** `Message`

---

### Step 2: Open Google Apps Script
1. In your Google Sheet, click **Extensions** in the top menu bar → **Apps Script**.
2. Delete any existing code in the editor, and paste the following script:

```javascript
function doPost(e) {
  try {
    var sheet = SpreadsheetApp.getActiveSpreadsheet().getActiveSheet();
    
    // Auto-create headers if sheet is empty
    if (sheet.getLastRow() === 0) {
      sheet.appendRow(["Timestamp", "Full Name", "Email", "Message"]);
      sheet.getRange(1, 1, 1, 4).setFontWeight("bold").setBackground("#e2e8f0");
    }
    
    var timestamp = e.parameter.timestamp || new Date().toLocaleString("en-IN", { timeZone: "Asia/Kolkata" });
    var name      = e.parameter.name || "N/A";
    var email     = e.parameter.email || "N/A";
    var message   = e.parameter.message || "N/A";
    
    sheet.appendRow([timestamp, name, email, message]);
    
    return ContentService.createTextOutput(JSON.stringify({ status: "success" }))
      .setMimeType(ContentService.MimeType.JSON);
  } catch (error) {
    return ContentService.createTextOutput(JSON.stringify({ status: "error", error: error.toString() }))
      .setMimeType(ContentService.MimeType.JSON);
  }
}
```

3. Click the **Save** icon (diskette icon) or press `Ctrl + S`.

---

### Step 3: Deploy as a Web App
1. At the top right of the Apps Script page, click the blue **Deploy** button → **New deployment**.
2. Click the gear icon next to "Select type" and choose **Web app**.
3. Fill in the fields:
   - **Description:** `Portfolio Form Webhook`
   - **Execute as:** `Me (your-email@gmail.com)`
   - **Who has access:** `Anyone` *(Crucial so visitors on your site can submit)*
4. Click **Deploy**.
5. Click **Authorize access**, choose your Google account, click **Advanced** → **Go to Untitled project (unsafe)**, and click **Allow**.
6. Copy the **Web app URL** (it looks like: `https://script.google.com/macros/s/AKfycbx.../exec`).

---

### Step 4: Paste the URL in `index.html`
1. Open `index.html`.
2. Locate line ~647:
   ```javascript
   var GOOGLE_SCRIPT_URL = "YOUR_GOOGLE_APPS_SCRIPT_URL_HERE";
   ```
3. Replace `"YOUR_GOOGLE_APPS_SCRIPT_URL_HERE"` with your copied Web App URL:
   ```javascript
   var GOOGLE_SCRIPT_URL = "https://script.google.com/macros/s/AKfycbx.../exec";
   ```
4. Save the file!

---

### Step 5: Test & Commit to Git
1. Open `index.html` in your browser and submit a test message in the contact form.
2. Check your Google Sheet — the new row will appear instantly! 🎉
3. Run:
   ```powershell
   git add index.html GOOGLE_SHEETS_DATABASE_SETUP.md
   git commit -m "feat: connect contact form to Google Sheets database"
   git push
   ```
