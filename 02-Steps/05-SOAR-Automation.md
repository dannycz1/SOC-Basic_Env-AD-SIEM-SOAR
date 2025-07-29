# Part 5 - SOAR Automation with Shuffle and Slack

## 🎯 Objective
Integrate Shuffle with Slack to automate the response to unauthorized logins detected by Splunk.

This step demonstrates **practical experience with SOAR automation**, which is critical for reducing incident response times and streamlining SOC workflows.

## 🛠️ Main Steps
1. Configured the Slack API and integrated it with Shuffle.
2. Built a playbook in Shuffle that:
   - Receives the Splunk alert.
   - Sends a notification to Slack.
   - Asks the SOC analyst for approval to disable the user.
3. Configured the workflow to disable the user in AD upon approval.

## 📷 Evidence
- Screenshot of the Shuffle playbook.
- Screenshot of Slack receiving the alert notification.
- Screenshot showing the user being disabled in AD.

## 🔗 Key Takeaways
- Hands-on experience integrating SIEM and SOAR platforms.
- Understanding of automated incident response workflows.
- Ability to design practical use cases for SOC environments.

## ✅ Result
When an unauthorized login is detected, the automated workflow sends a Slack notification and, upon analyst approval, disables the user account in AD.  
This reduces response time and simulates a real-world SOC analyst workflow.
