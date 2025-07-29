# Part 5 - SOAR Automation with Shuffle and Slack

## 🎯 Objective
Integrate Shuffle with Slack to automate the response to unauthorized logins.

## 🛠️ Main Steps
1. Configure the Slack API and integrate it with Shuffle.
2. Create a playbook in Shuffle that receives the Splunk alert and sends a notification to Slack.
3. Configure the workflow so that, if the analyst approves, the user is disabled in Active Directory.

## 📷 Evidence
- Screenshot of the playbook in Shuffle.
- Slack notification.
- Evidence of the user being disabled in AD.

## ✅ Result
When an unauthorized login occurs, the automation workflow sends an alert to Slack and allows the user to be automatically disabled in AD.
