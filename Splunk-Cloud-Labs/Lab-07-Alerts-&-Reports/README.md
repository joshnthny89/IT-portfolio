# 🚨 Lab 07 – Alerts & Reports

## Objective

Learn how to create scheduled reports and alerts in Splunk Cloud to automate the monitoring of machine data. This lab demonstrates how searches can be reused to notify analysts of important events and generate reports without requiring manual intervention, improving both efficiency and situational awareness.

---

## Skills Practiced

- Scheduled Searches
- Alert Configuration
- Report Creation
- Search Processing Language (SPL)
- Security Monitoring
- SIEM Operations

---

## Tools Used

- Splunk Cloud Platform
- Search & Reporting App
- Reports
- Alerts

---

# Lab Walkthrough

## Scenario

After creating searches, statistical reports, and dashboards in previous labs, the next step is automating those searches. Rather than manually checking dashboards throughout the day, analysts can configure reports and alerts that run automatically and notify them when specific conditions are met. This helps reduce response time and ensures important events are not overlooked.

---

## Step 1 – Run a Search

Opened the **Search & Reporting** application and executed a search that returned meaningful event data.

Example:

```spl
index=* | stats count by host
```

This search served as the foundation for creating both a report and an alert.

### Screenshot

<img width="1277" height="711" alt="image" src="https://github.com/user-attachments/assets/5d37da6a-0536-4321-9b55-ccbe6002aae4" />


**Caption**

<sub><em>Executed a search that produced meaningful results suitable for automation through reports and alerts.</em></sub>

---

## Step 2 – Save the Search as a Report

Selected **Save As → Report** and assigned the report a descriptive name.

Reports allow commonly used searches to be saved and rerun without recreating the SPL query each time.

### Screenshot

<img width="1136" height="323" alt="image" src="https://github.com/user-attachments/assets/29429624-a54a-4bcc-bd5d-2fedd24b6367" />
<img width="557" height="368" alt="image" src="https://github.com/user-attachments/assets/45756518-92f2-4d8a-bef2-79c170903acf" />


**Caption**

<sub><em>Saved the completed search as a reusable report for future analysis and monitoring.</em></sub>

---

## Step 3 – Configure a Scheduled Report

Configured the report to run automatically on a scheduled interval.

Scheduling reports enables analysts to receive updated search results without manually executing the search each day.

### Screenshot

<img width="797" height="672" alt="image" src="https://github.com/user-attachments/assets/a99a7dc9-14b6-4281-851b-39149e80b848" />


**Caption**

<sub><em>Configured the report to run automatically, reducing the need for manual searches.</em></sub>

---

## Step 4 – Create an Alert

Created an alert using the same search.

Configured the alert to trigger when specified search conditions were met, allowing Splunk to automatically notify analysts when important activity is detected.

### Screenshot

<img width="1130" height="265" alt="image" src="https://github.com/user-attachments/assets/ccb43335-14df-4af3-8f4a-7eea8588ae1e" />
<img width="794" height="832" alt="image" src="https://github.com/user-attachments/assets/5249c23d-d8b8-46d6-ac9d-04ec85e58f34" />


**Caption**

<sub><em>Created an alert that automatically monitors search results and triggers when predefined conditions are met.</em></sub>

---

## Step 5 – Configure Alert Actions

Reviewed the available alert actions and configured the appropriate notification settings.

Depending on the environment, alert actions may include:

- Email notifications
- Triggered actions
- Webhooks
- Running scripts
- Creating notable events

Automated alert actions help reduce response times by notifying analysts immediately when important events occur.

### Screenshot

<img width="795" height="773" alt="image" src="https://github.com/user-attachments/assets/050dbbb5-da11-4fe6-bea3-7e5033fda025" />


**Caption**

<sub><em>Configured alert actions to automate notifications when specified search conditions are detected.</em></sub>

---

## Step 6 – Review Saved Reports and Alerts

Reviewed the completed report and alert to verify that both were successfully saved and configured.

Confirmed that the saved objects were available for future monitoring and could be modified as operational requirements change.

### Screenshot

<img width="1115" height="433" alt="image" src="https://github.com/user-attachments/assets/473c7057-49d2-449e-9318-cee5ba108f60" />
<img width="1132" height="633" alt="image" src="https://github.com/user-attachments/assets/5c5a0ddd-9de7-4a7d-8b93-2475169ee66e" />
<img width="1137" height="252" alt="image" src="https://github.com/user-attachments/assets/825fd4ad-c029-4d60-ae7f-11dd34f784e2" />


**Caption**

<sub><em>Verified that the report and alert were successfully created and ready for automated monitoring.</em></sub>

---

## What I Learned

This lab demonstrated how Splunk Cloud can automate routine monitoring tasks through scheduled reports and alerts. Rather than manually performing the same searches throughout the day, I learned how saved searches can generate reports on a schedule and trigger alerts when specific conditions are met. These capabilities help security teams monitor systems more efficiently, improve response times, and ensure important events receive timely attention.

---

## Skills Learned

- Creating scheduled reports
- Configuring automated alerts
- Saving reusable searches
- Scheduling report execution
- Configuring alert conditions
- Understanding automated monitoring workflows
- Supporting proactive security monitoring
