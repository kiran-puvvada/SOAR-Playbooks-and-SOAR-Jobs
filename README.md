
1.Log Stoppage Automation:

This project automates the monitoring of log sources to ensure continuous data ingestion.   
The Problem: Stale cases accumulate because analysts lack visibility on when ingestion resumes, leading to manual verification backlogs.   The Solution: A Scheduled SOAR Job that identifies open log stoppage cases and queries Chronicle via UDM to verify if logs have resumed.

Outcome: Automatically closes cases when logs are detected or sends re-escalation reminders every 3 hours if they are still missing.  
 
2. Phishing Investigation & Response :
A modernized playbook that transitions phishing response from a manual process to an AI-assisted, automated workflow.  
The Problem: Manual header analysis and the lack of bulk email deletion capabilities created significant bottlenecks in Mean Time to Respond (MTTR).   
The Solution: Integration with ActOn Investigator for AI-driven verdicts and Google Threat Intelligence (GTI) for enrichment.   
Outcome: Enables Bulk Remediation, allowing analysts to instantly purge malicious emails from all recipient inboxes across G Suite or Office 365.   

3. Playbook Failure Reporting Job:
A centralized monitoring tool designed to ensure the health and reliability of all automations within the environment.   
The Problem: No native mechanism exists to detect failed playbooks, forcing analysts to manually check every case for automation errors.   The Solution: A Python-based scheduled job that iterates through all cases to identify playbooks with a "Failed" status.   
Outcome: Extracts specific error messages from the case wall and delivers a consolidated failure report to the SOC team for rapid troubleshooting.  
