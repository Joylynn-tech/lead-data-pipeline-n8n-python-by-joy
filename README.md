🔄 End-to-End Lead Data Pipeline with n8n and Python

A fully automated data pipeline that extracts, cleans, analyzes, and generates business deductions from 1,000 leads running on a daily schedule with zero manual intervention.
Built by Joylynn Mumbi Ngari | @joywithdata

📌 Project Overview

Small businesses waste hours manually tracking leads across spreadsheets with no visibility into which channels convert best. This project solves that by building a fully automated pipeline that does the heavy lifting every day at 8:00 AM  no human needed.

❗ Problem Statement

Sales teams lose valuable time and revenue to fragmented lead management processes. Without an automated system, leads are manually logged across disconnected tools, creating delays, data gaps, and missed follow-up opportunities. There is no real time visibility into pipeline health or lead source performance, making it impossible to identify which channels drive the highest conversions. High potential leads go cold due to the absence of priority flagging or automated outreach triggers

✅ Solution

A 5-node automated pipeline built in n8n:

🛠️ Tech Stack

n8n Cloud-Workflow automation & scheduling
Google Sheets-Data source
Python (n8n Code node)-Cleaning, EDA, deductions
GitHub-Version control & portfolio

📊 Dataset

Synthetic dataset of 1,000 leads generated with Python simulating a legal services lead generation business.


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

1.Total Leads-1,000 across 9 sources

2.Best Lead Source-LinkedIn — 137 leads

3.Best Converting Source-Referral — highest Won rate

4.Leads Needing Follow-up-324 stuck in New Lead stage

5.Conversion Rate-7.2% — above 2-5% industry average

6.Total Won Revenue-$1,983,085 from 72 deals

7.Recommendation-Increase Referral budget. Follow up on 324 stale leads.

💡 Skills Demonstrated

1.Workflow Automation (n8n)

2.Python scripting (cleaning, EDA, deductions)

3.Data cleaning and validation

4.Exploratory Data Analysis

5.Business insight generation

6.Synthetic data generation

👩🏾‍💻 About Me

Hi! I'm Joylynn, a data analyst based in Nairobi, Kenya with 3+ years of experience in supply chain data analysis. I'm passionate about using data and automation to solve real business problems.

📸 Follow my learning journey: @joywithdata

💼 Open to freelance data analyst and automation projects

Built with 💛 by Joylynn Mumbi Ngari
