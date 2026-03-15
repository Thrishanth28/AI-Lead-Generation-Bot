# AI-Lead-Generation-Bot
🎯 AI Lead Generation Bot — n8n Automation Workflow
An automated cold outreach system built with n8n, Google Gemini, and Gmail. Fill a simple form with lead details, and AI instantly writes a personalized cold email and sends it automatically — plus a confirmation copy to you.

🚀 What It Does
In just one form submission, this workflow automatically:

📋 Collects your details + lead details via a clean n8n form
🧠 Sends everything to Google Gemini to write a personalized cold email
📤 Sends the cold email directly to the lead's inbox
✅ Sends a confirmation copy to you with full email summary


📸 Workflow Overview
Lead Form (n8n Form Trigger)
        │
        ▼
Generate Cold Email (Google Gemini — writes personalized outreach)
        │
        ▼
Send Cold Email to Lead (Gmail — delivers to lead's inbox)
        │
        ▼
Send Confirmation to You (Gmail — summary copy for your records)

📋 Form Fields
FieldExampleYour NameThrishanth ReddyYour RoleAI Automation DeveloperYour Service / Offern8n automation workflowsLead NameRahul SharmaLead Emailrahul@company.comLead CompanyTechStartup Pvt LtdLead Role / PositionFounder / CTOWhy are you reaching out?Their team wastes time on manual tasks

🛠️ Tools & Technologies
ToolPurposen8nWorkflow automation platformGoogle Gemini (PaLM API)AI cold email writingGmail API (OAuth2)Send email to lead + confirmation to youn8n Form TriggerClean input form — no coding needed

📧 Sample AI Generated Email
Subject: Saving TechStartup 10 hours/week

Hi Rahul,

I noticed TechStartup is scaling fast — but fast
growth usually means more manual work piling up.

I help founders like you automate repetitive
workflows using n8n — things like emails, invoices,
data entry — all on autopilot.

Recently helped a client save 10+ hours/week
doing exactly this.

Would you be open to a 15-minute call this week?

Best,
Thrishanth Reddy
AI Automation Developer

⚙️ Setup Instructions
Prerequisites

n8n installed (cloud or self-hosted)
Google Gemini API key
Gmail OAuth2 credentials configured in n8n

Steps

Clone this repo

bash   git clone https://github.com/Thrishanth28/n8n-automation-agents.git

Import the workflow into n8n

Open your n8n dashboard
Go to Workflows → Import from File
Select AI_Lead_Generation_Bot.json


Configure credentials in n8n

Add your Google Gemini API credentials
Add your Gmail OAuth2 credentials


Test the workflow

Click Execute Workflow
Fill the form — use YOUR OWN email as Lead Email for testing
Check inbox — you should receive the cold email + confirmation ✅


Activate the workflow

Toggle the workflow to Active ✅




🔧 Customization
Change email tone:
In the Generate Cold Email node, update the system prompt tone:
Sound more formal / casual / friendly
Change email length:
Update this line in the prompt:
Maximum 150 words in the email body
Change to any word count you prefer.
Change confirmation email recipient:
In the Send Confirmation to You node, update the To field:
your-email@gmail.com
Add follow-up automation:
Connect a Wait node after confirmation → add a second Gmail node
to send a follow-up email after 3–5 days automatically.

💡 Real World Use Cases

🧑‍💻 Freelancers — Reach out to potential clients at scale
🎓 Students — Send personalized internship applications
📱 Startups — Automate sales outreach completely
🏢 Agencies — Pitch services to new businesses daily
💼 Job seekers — Cold email HR managers and founders directly


🔐 Security Note

⚠️ Never commit real API keys or credentials to GitHub.
All credentials in this repo are placeholders.
Add your real keys only inside your n8n credential manager.


🙋‍♂️ Built By
S. Thrishanth Reddy — AI Automation Developer
Skills: n8n · Prompt Engineering · HTML/CSS · Python · SQL
📎 LinkedIn | 🔗 GitHub

📄 License
MIT License — free to use, modify, and share!
