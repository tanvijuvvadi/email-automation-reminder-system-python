# 📧 Email Automation & Reminder System

## 🚀 Project Overview

The **Email Automation & Reminder System** is a Python-based application designed to automate repetitive email communication tasks such as sending reminders, follow-ups, and notifications.

This system reads contact data from CSV files, personalizes email templates, schedules reminders, sends emails using SMTP, and tracks delivery status with logs and reports.



## ❗ Problem Statement

In many organizations, sending emails manually:

* Consumes time ⏳
* Leads to missed follow-ups ❌
* Lacks tracking and reporting 📉

This project solves these issues by automating the entire workflow.


## 💡 Industry Relevance

This system can be used by:

* 👨‍💼 HR Teams → Interview reminders
* 📢 Marketing Teams → Campaign emails
* 🎓 Trainers → Session reminders
* 💰 Finance Teams → Payment reminders
* 📊 Operations Teams → Task notifications


## ✨ Features

* 📬 Automated email sending
* ⏰ Scheduled reminders
* 👤 Personalized email templates
* 🧾 CSV-based contact management
* 📊 Delivery status tracking (Sent/Failed)
* 🪵 Logging system for monitoring
* 📁 Report generation (CSV)
* 🛡️ Secure credentials using environment variables
* 🧪 Dry-run mode (test without sending real emails)


## 🛠️ Tech Stack

* **Python**
* **Pandas**
* **smtplib (SMTP)**
* **email.message**
* **schedule**
* **datetime**
* **python-dotenv**
* **logging**


## 📁 Project Structure

Email-Automation-Reminder-System/
│
├── data/               # Input CSV files (contacts, reminders)
├── templates/          # Email templates
├── src/                # Python modules (optional for scaling)
├── outputs/            # Generated reports
├── logs/               # Log files
├── images/             # Screenshots for documentation
├── docs/               # Additional documentation
├── main.py             # Main execution file
├── requirements.txt    # Dependencies
├── .gitignore          # Ignored files
└── README.md           # Project documentation


## ⚙️ Installation & Setup

### 1️⃣ Clone Repository

bash
git clone https://github.com/your-username/email-automation-reminder-system.git
cd email-automation-reminder-system


### 2️⃣ Create Virtual Environment

bash
python -m venv venv


### 3️⃣ Activate Environment

**Windows:**
bash
venv\Scripts\activate


**Mac/Linux:**

bash
source venv/bin/activate


### 4️⃣ Install Dependencies

bash
pip install -r requirements.txt


## 🔐 Environment Variables Setup

Create a `.env` file in the root directory:


EMAIL=your_email@gmail.com
PASSWORD=your_app_password


⚠️ **Important:**

* Use Gmail App Password (not your real password)
* Do NOT upload `.env` file to GitHub


## ▶️ How to Run the Project

### Run in Dry-Run Mode (Safe Testing)

bash
python main.py


Output:

[DRY RUN] Email to john@example.com
Report generated.


### Run in Real Mode

1. Set:

DRY_RUN = False


2. Run:

python main.py


## 📄 Input Files

### contacts.csv


name,email
John,john@example.com
Alice,alice@example.com


### reminders.csv

time
18:30


### email_template.txt

Hello {{name}},

This is a reminder for your scheduled task.

Thanks,
Team



## 📊 Output

### Generated Files:

* `logs/email.log` → Logs of sent/failed emails
* `outputs/report.csv` → Email delivery report

## 🧪 Virtual Simulation

* Use dummy emails ([example@gmail.com](mailto:example@gmail.com))
* Enable `DRY_RUN = True`
* Verify logs and reports without sending real emails



## 🔒 Security Best Practices

* ❌ Never upload `.env` file
* ❌ Never expose passwords
* ✅ Use `.env.example` file
* ✅ Add `.env` in `.gitignore`


## 📈 Future Enhancements

* FastAPI backend
* Web dashboard (Streamlit/React)
* Email tracking (opened/read)
* Database integration (PostgreSQL)
* Bulk email campaigns
* Retry mechanism for failed emails


## 🎯 Learning Outcomes

* Python automation
* Email protocols (SMTP)
* Scheduling systems
* Data handling using Pandas
* Logging & monitoring
* Real-world workflow design




