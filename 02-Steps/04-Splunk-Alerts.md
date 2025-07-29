# Part 4 - Splunk Setup & Alerts

## 🎯 Objective
Deploy Splunk on Ubuntu, ingest Windows security logs from the domain controller, and create an alert to detect unauthorized successful logins.

This step demonstrates practical SIEM configuration and log analysis skills, essential for a SOC Analyst to detect suspicious authentication events in Active Directory environments.

## 🛠️ Main Steps
1. Installed Splunk Enterprise on Ubuntu (Vultr).
2. Configured Universal Forwarder on Windows Server (DC01) to send Security Event Logs.
3. Verified ingestion of EventCode 4624 (successful logins) in Splunk.
4. Created a correlation search to detect successful logins from unauthorized accounts.

## 📷 Evidence
- Splunk search showing ingested Windows events.  
- Alert rule configured in Splunk (screenshot of correlation search).  

## 🔗 Key Takeaways
- Understanding of SIEM log ingestion and configuration.  
- Knowledge of Windows Event Codes relevant to authentication.  
- Practical experience creating detection rules aligned with SOC use cases.

## ✅ Result
Splunk ingests authentication events from the domain controller and triggers an alert upon detecting unauthorized successful logins.  
This alert will serve as the detection source for the SOAR automation in the next phase.
