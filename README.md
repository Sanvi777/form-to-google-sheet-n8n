# Form to Google Sheets Automation 📩

A simple **n8n automation workflow** that collects user requests through a web form and automatically stores the submitted data in a **Google Sheet**.

## 📌 Project Overview

This project creates a support/request form where users can enter:

- Name
- Email
- Request

After the user submits the form, **n8n automatically receives the submission and adds it as a new row in Google Sheets**.

## 🔄 Workflow

```text
User
  ↓
Support Form
  ↓
On Form Submission (n8n)
  ↓
Append Row in Google Sheets
  ↓
Google Spreadsheet
✨ Features
📝 Simple support request form
📧 Collects user name and email
💬 Collects the user's request/message
⚡ Automatically processes form submissions
📊 Saves submissions directly to Google Sheets
🔐 Uses Google authentication for Sheets access
🔄 Adds every new submission as a separate row
🤖 Built using n8n workflow automation
🛠️ Technologies Used
n8n – Workflow automation
n8n Form Trigger – Creates and handles the form
Google Sheets – Stores form submissions
Google Cloud – Used for Google API and OAuth authentication
📋 Form Fields

The form contains the following fields:

Field	Description
Name	Name of the person submitting the request
Email	Email address of the user
Request	Support request or message
📊 Google Sheets

The submitted information is stored in Google Sheets in the following format:

Name	Email	Request
Sanvi	sanvisharma185...	Send me more cookies
Sarah	sarahkrishan963...	Hello, Teach me

Every time a user submits the form, a new row is automatically added to the sheet.

⚙️ How It Works
1. User submits the form

The user opens the n8n-generated form and enters their:

Name
Email
Request
2. n8n receives the submission

The On Form Submission node is triggered when the user clicks the Submit button.

3. Data is sent to Google Sheets

The submitted data is passed to the Google Sheets node.

4. A new row is added

The Append Row in Sheet operation automatically adds the information to the connected Google Spreadsheet.

🔐 Google Authentication

Google Sheets authentication is configured in n8n using Google credentials/OAuth.

The required Google Sheets API is enabled through the Google Cloud Console.

🚀 Setup
Install and start n8n.
Create a new workflow.
Add an On Form Submission node.
Create the required form fields.
Add a Google Sheets node.
Select Append Row as the operation.
Connect your Google account using OAuth credentials.
Select the Google Spreadsheet and Sheet.
Map the form fields to the spreadsheet columns.
Activate/publish the workflow.
Submit the form and check the Google Sheet.
🎯 Use Cases

This workflow can be used for:

Support request collection
Contact forms
Feedback forms
Student queries
Customer requests
Complaint collection
Simple lead collection
Internal request management
📁 Project Structure
Form-to-Google-Sheet/
│
├── README.md
└── workflow.json

workflow.json can contain the exported n8n workflow if you choose to include it in the repository.

📸 Project Preview

The project includes:

A support request form
An n8n automation workflow
A Google Sheet containing submitted requests
👩‍💻 Author

Sanvi Sharma

GitHub: Sanvi777
