# Part 4 - Splunk Setup & Alerts

## 🎯 Objective
Configure Splunk to receive logs from the domain controller and create an alert to detect unauthorized logins.

## 🛠️ Main Steps
1. Install Splunk on Ubuntu (Vultr).
2. Configure the Universal Forwarder on Windows Server (AD).
3. Validate event ingestion using a Splunk search.
4. Create a basic alert to detect successful unauthorized logins.

## 📷 Evidence
- Splunk receiving events (screenshot of the search).
- Alert configuration (screenshot of the created rule).

## ✅ Result
Splunk ingests events correctly and generates an alert when an unauthorized login occurs.
