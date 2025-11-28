# Playwright_Python
# Bank App Automation Framework

Automated web and API testing framework for a **demo banking application** using **Python, Playwright, and Pytest**.

---

## 🛠 Tech Stack

- **Language:** Python  
- **Test Automation:** Playwright  
- **Test Framework:** Pytest  
- **HTTP Requests / API Testing:** requests  
- **Data Management:** JSON / external test data  

---

---
## 📁 Project Structure
project/
├── pages/
│ ├── base_page.py
│ ├── login_page.py
│ ├── dashboard_page.py
│ ├── transfer_page.py
│ └── transactions_page.py
├── tests/
│ ├── test_login.py
│ ├── test_fund_transfer.py
│ ├── test_download_statement.py
│ └── test_api_ui_balance_check.py
├── utils/
│ ├── config.py
│ └── testdata.py
├── conftest.py
└── requirements.txt

---

## ⚡ Features

### UI Automation
- Login functionality  
- Fund transfer between accounts  
- Viewing transaction history  
- Downloading bank statements  

### API Testing
- Integration of API response validation with UI tests  

### Framework Features
- **Page Object Model (POM):** Reusable page classes  
- **Data-driven tests:** External JSON test data  
- **Pytest Fixtures:** Browser context, isolated pages  
- **File Download Handling:** Validate downloaded statements  
- **Headless & Headed Execution:** Supports both  

---

## 📌 Installation
1. Clone the repository:
```bash
git clone https://github.com/yourusername/bank-app-automation.git
cd bank-app-automation
Create a virtual environment (optional but recommended):

python -m venv venv
# Linux / Mac
source venv/bin/activate
# Windows
venv\Scripts\activate```


2. Install dependencies:

```pip install -r requirements.txt
playwright install
```

#🚀 Running Tests

Run all tests:

pytest


Run a specific test:

pytest tests/test_login.py

📂 Test Data

All test data is stored in utils/testdata.py. Example structure:

{
    "valid_user": {
        "username": "admin",
        "password": "admin123"
    },
    "transfer": {
        "to_account": "1234567890",
        "amount": "1000",
        "remark": "Test Transfer"
    }
}

