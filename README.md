🔄 End-to-End Lead Data Pipeline with n8n and Python

A fully automated data pipeline that extracts, cleans, analyzes, and generates business deductions from 1,000 leads running on a daily schedule with zero manual intervention.
Built by Joylynn Mumbi Ngari | @joywithdata

📌 Project Overview

Small businesses waste hours manually tracking leads across spreadsheets with no visibility into which channels convert best. This project solves that by building a fully automated pipeline that does the heavy lifting every day at 8:00 AM  no human needed.

❗ Problem Statement

Manual lead tracking is time-consuming and error-prone
No visibility into which lead sources convert best
Leads sit untouched with no system to flag them
Revenue attribution is unclear making budget decisions difficult
Reports take hours to produce manually each week

✅ Solution

A 5-node automated pipeline built in n8n:

🛠️ Tech Stack

n8n Cloud-Workflow automation & scheduling
Google Sheets-Data source
Python (n8n Code node)-Cleaning, EDA, deductions
GitHub-Version control & portfolio

📊 Dataset

Synthetic dataset of 1,000 leads generated with Python simulating a legal services lead generation business.

📊Columns

Description
Lead ID
Unique identifier
Full Name
Contact name
Email / Phone
Contact details
State
US state
Lead Source
Google Ads, LinkedIn, Referral, etc.
Service Interest
Personal Injury, SSDI, Mass Tort, etc.
Pipeline Stage
New Lead → Contacted → Qualified → Won / Lost
Assigned Rep
Auto-assigned based on lead source
Date Created
Last 6 months
Estimated Revenue
Dollar value for Won deals only

🔁 Pipeline Walkthrough

1. Schedule Trigger
Runs automatically every day at 8:00 AM. No manual action needed.

2. Data Extraction
n8n connects to Google Sheets via OAuth2 and pulls all 1,000 rows automatically.

3. Data Cleaning (Python)
Strips whitespace from all text fields
Standardizes Lead Source and Pipeline Stage to title case
Handles missing email addresses
Converts Estimated Revenue to float

4. EDA (Python)
Counts leads by source, pipeline stage, and assigned rep
Calculates total revenue from Won deals
Identifies best converting sources

5. Automated Deductions (Python)
Generates business insights automatically — no manual interpretation needed.

📈 Key Findings

Total Leads-1,000 across 9 sources

Best Lead Source-LinkedIn — 137 leads

Best Converting Source-Referral — highest Won rate

Leads Needing Follow-up-324 stuck in New Lead stage

Conversion Rate-7.2% — above 2-5% industry average

Total Won Revenue-$1,983,085 from 72 deals

Recommendation-Increase Referral budget. Follow up on 324 stale leads.

💡 Skills Demonstrated

Workflow Automation (n8n)

Python scripting (cleaning, EDA, deductions)

Data cleaning and validation

Exploratory Data Analysis

Business insight generation

Synthetic data generation

👩🏾‍💻 About Me

Hi! I'm Joylynn, a data analyst based in Nairobi, Kenya with 3+ years of experience in supply chain data analysis. I'm passionate about using data and automation to solve real business problems.

📸 Follow my learning journey: @joywithdata
💼 Open to freelance data analyst and automation projects
Built with 💛 by Joylynn Mumbi Ngari
