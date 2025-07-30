# Part 4 - Splunk Setup & Alerts

## 🎯 Objective
Deploy Splunk on Ubuntu, ingest Windows security logs from the domain controller, and create an alert to detect unauthorized successful logins.

This step demonstrates practical SIEM configuration and log analysis skills, essential for a SOC Analyst to detect suspicious authentication events in Active Directory environments.

## 🛠️ Main Steps
### 1. Installed Splunk Enterprise on Ubuntu.
  - First, we register with Splunk by going to Platform -> Products -> Free Trials & Downloads -> Splunk Enterprise and copying the link. Then we download Splunk on Ubuntu.
  - Next, we need to run the binary called "splunk", to do this we install the .deb package, then we search for and run the binary to finish the Splunk installation:
```bash
	dpkg -i <downloadfile.deb>
	cd /opt/splunk/bin
	./splunk start
```
  We observe the message after installation, this data will help us log in to Splunk in the browser.
  ![deploy-panel](../03-Evidences/step_4-url_web_interface_address.png)

  - We also need to allow port 8000 on Ubuntu: access to Splunk web console (also in Azure NGS, but at this point that has already been done)
```bash
ufw allow 8000
```
  - I now have access to Splunk from my personal laptop.
  ![deploy-panel](../03-Evidences/step_4-splunk_web_access.png)
    
### 2. Configured Universal Forwarder on Windows Server (DC01) to send Security Event Logs.
### 3. Verified ingestion of EventCode 4624 (successful logins) in Splunk.
### 4. Created a correlation search to detect successful logins from unauthorized accounts.

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
