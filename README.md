# n8n
📦 Automated Shipment Plan Email Workflow
This project implements an automated workflow for generating and sending shipment plans via email based on data in a PostgreSQL database.

✅ Overview
This workflow:

Runs on a scheduled trigger.

Executes a PostgreSQL query to retrieve shipment plan data.

Formats the data into CSV.

Checks if data exists:

If yes: Exports the shipment plan and sends it via Gmail.

If no: Sends a “No Data” notification email.

⚙️ Workflow Steps
Step	Description
Schedule Trigger	Runs daily/weekly (as configured) to start the workflow.
PostgreSQL Query	Fetches shipment plan data from the database.
Format Data for CSV	Converts query result into CSV format for sharing.
Check If Data Exists	Branches logic based on whether results are empty or not.
Export Shipment Plan	Saves the CSV if data exists.
Gmail Integration	Sends an email with the CSV attachment (or notification if no data exists).

🗺️ Workflow Diagram

(Replace your-workflow-image.png with your actual file name.)

💻 Technologies Used
PostgreSQL

Custom scripting for CSV formatting

Gmail API / Integration

Automation platform (e.g. n8n, Make.com, Zapier – specify which one you used)

🚀 Usage
Clone this repository.

Review the workflow image to understand the steps.

Adapt the database query and email details to your environment.
