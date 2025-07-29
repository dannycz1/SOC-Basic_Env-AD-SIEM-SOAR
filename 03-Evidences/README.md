
# Project Evidences

## 📖 Purpose
This folder contains all the key screenshots and artifacts generated during the project.  
Each evidence is referenced in the corresponding step documentation under `/02-Steps/`.

## 📂 Structure
| File Name              | Description                                              | Related Step |
|------------------------|----------------------------------------------------------|--------------|
| ad_users.png           | Active Directory user accounts created.                 | Part 3       |
| ad_domain_join.png     | Endpoint successfully joined to the AD domain.          | Part 3       |
| splunk_search.png      | Splunk search showing ingested authentication events.   | Part 4       |
| splunk_alert.png       | Configured Splunk alert for unauthorized logins.        | Part 4       |
| shuffle_playbook.png   | Automation playbook created in Shuffle.                 | Part 5       |
| slack_notification.png | Slack notification received after alert triggering.     | Part 5       |
| ad_user_disabled.png   | User account disabled in AD after automated response.   | Part 5       |

## 📌 How to Use
Each Markdown file in `/02-Steps/` links to these evidences using relative paths, for example:

```markdown
![Splunk Alert](../03-Evidences/splunk_alert.png)
