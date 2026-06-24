# 🏨 Restful Booker API Testing

![Postman](https://img.shields.io/badge/Postman-API_Testing-FF6C37?logo=postman&logoColor=white)
![Newman](https://img.shields.io/badge/Newman-Test_Runner-00A98F)
![Node.js](https://img.shields.io/badge/Node.js-Required-339933?logo=node.js&logoColor=white)
![Status](https://img.shields.io/badge/Execution-Completed-success)
![Failed Assertions](https://img.shields.io/badge/Failed_Assertions-5-red)

A complete REST API testing project for the Restful Booker public API using Postman, Newman, and Node.js.

The test suite validates the end-to-end booking workflow, covering booking creation, retrieval, authentication, update, partial update, and deletion, with automated execution and detailed HTML reporting.
________________

# 🔗 Base URL
"https://restful-booker.herokuapp.com"

________________
## 🛠️ Tools & Technologies

| Tool | Purpose |
|------|----------|
| 📮 Postman | API Development & Testing |
| 🚀 Newman | Command Line Collection Runner |
| 🟢 Node.js | Runtime Environment |
| 📊 HTML Extra Reporter | Detailed Test Reporting |
| 📜 JavaScript | Test Script Development |

________________

# 📂 Project Structure
# File	Description
📮 Collection	Stores the Postman collection file (API_Testing.postman_collection.json)

⚙️ Environment	Contains environment variables used during execution (API_Testing.postman_environment.json)

📊 Reports	Generated Newman HTML execution reports (Newman_Report.html)

📸 Screenshots	Contains dashboard and execution result screenshots (Newman_Run_Dashboard.png)

📄 README.md	Project documentation, setup instructions, and execution details

________________

# 🔄 Test Workflow
Get Booking IDs
        ↓
Create Booking
        ↓
Get Booking
        ↓
Create Token
        ↓
Update Booking
        ↓
Partial Update Booking
        ↓
Delete Booking

________________

# ✅ API Endpoints Covered
# Method	Endpoint	Purpose
GET	/booking	Get Booking IDs

POST	/booking	Create Booking

GET	/booking/{id}	Get Booking Details

POST	/auth	Generate Token

PUT	/booking/{id}	Update Booking

PATCH	/booking/{id}	Partial Update

DELETE	/booking/{id}	Delete Booking

________________

# 🧪 Validation Performed
• Functional Validation

• Status Code Verification

• Response Body Verification

• Authentication Validation

• Data Integrity Check

• Automation Validation

• Dynamic Variable Extraction

• Environment Variable Usage

• Chained API Requests

• Automated Assertions

• Performance Validation

• Response Time Monitoring

• Payload Verification

________________

 ## 📊 Newman Execution Report

| Category | Result |
|-----------|----------|
| 🔄 Iterations Executed | 1 |
| 📨 Requests Executed | 8 |
| ✅ Assertions Executed | 62 |
| 🟢 Assertions Passed | 57 |
| 🔴 Assertions Failed | 5 |
| ⏭️ Tests Skipped | 0 |
| ⚡ Average Response Time | 569 ms |
| ⏱️ Execution Duration | 5.3 s |
| 📦 Total Data Received | 40.97 KB |

________________

# 📸 Execution Dashboard
<img width="616" height="608" alt="Newman Run Dashboard_Screenshot" src="https://github.com/user-attachments/assets/267ac011-cc09-40b2-910c-ef2dbda7d31d" />

________________

# ⚠️ Failed Assertions Analysis
• Create Booking

Expected Status Code: 201

Actual Status Code: 200

• Create Booking

Expected: depositpaid = true

Actual: depositpaid = false

• Get Booking

Expected: depositpaid = true

Actual: depositpaid = false

• Create Token

Expected Status Code: 201

Actual Status Code: 200

• Delete Booking

Expected Status Code: 200

Actual Status Code: 201

# Root Cause

The failures are caused by assertion expectation mismatches rather than endpoint failures. The APIs responded successfully, but some expected values in the test scripts did not match the actual API responses.

________________

# ▶️ Run This Project
# Step	Command
📦 Install Newman	npm install -g newman

📊 Install HTML Reporter	npm install -g newman-reporter-htmlextra

🚀 Execute Collection	newman run API_Testing.postman_collection.json -e API_Testing.postman_environment.json -r cli,htmlextra

________________

# 📈 Key Achievements

✔ End-to-End API Automation

✔ Dynamic Data Handling

✔ Authentication Testing

✔ CRUD Operations Validation

✔ Automated Newman Execution

✔ HTML Report Generation

✔ API Response Verification

________________

# Shanjana Tanjim

💡Interested in Software Quality Assurance

________________

# 📌 About This Project

A hands-on API automation testing project built to validate the complete booking workflow of the Restful Booker API. The project demonstrates the use of Postman collections, automated Newman execution, response validation, and detailed HTML reporting for effective API quality assurance.







