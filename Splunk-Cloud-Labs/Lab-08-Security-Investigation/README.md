# 🛡️ Lab 08 – Security Investigation

## Objective

Apply the skills developed throughout the previous Splunk Cloud labs to investigate a collection of machine data using Search Processing Language (SPL). This lab brings together searching, field analysis, statistical commands, dashboards, and alerts to simulate the workflow of a Security Operations Center (SOC) analyst investigating suspicious activity.

---

## Skills Practiced

- Security Investigation
- Search Processing Language (SPL)
- Event Analysis
- Field Analysis
- Statistical Analysis
- Dashboard Review
- Security Monitoring
- Incident Documentation
- SIEM Operations

---

## Tools Used

- Splunk Cloud Platform
- Search & Reporting App
- Dashboards
- Reports
- Alerts

---

# Lab Walkthrough

## Scenario

Throughout the previous labs, I learned how to search indexed data, work with extracted fields, summarize information using statistical commands, build dashboards, and configure alerts. In this capstone lab, I applied those skills together to investigate a dataset in Splunk Cloud using a structured analytical workflow similar to one used by SOC analysts.

---

## Step 1 – Begin the Investigation

Opened the **Search & Reporting** application and reviewed the available machine data before beginning the investigation.

Performed an initial search to establish a baseline of available events.

```spl
index=*
```

Starting with a broad search helps determine what data is available before narrowing the investigation.

### Screenshot

<img width="1143" height="890" alt="image" src="https://github.com/user-attachments/assets/65c6b088-2634-4815-8aa3-1f697c348526" />


**Caption**

<sub><em>Began the investigation by reviewing indexed machine data and establishing a baseline search.</em></sub>

---

## Step 2 – Narrow the Search

Applied additional search criteria to reduce the number of returned events and focus on relevant activity.

Examples may include filtering by:

- Host
- Source
- Sourcetype
- Keyword
- Time Range

Filtering unnecessary data allows analysts to investigate more efficiently.

### Screenshot

<img width="1280" height="911" alt="image" src="https://github.com/user-attachments/assets/60d2ed78-44da-4c93-bb03-7e7e8816b733" />
<img width="1144" height="863" alt="image" src="https://github.com/user-attachments/assets/4f16e922-8401-4ba1-9076-613b65360bea" />


**Caption**

<sub><em>Refined the search results to isolate the events most relevant to the investigation.</em></sub>

---

## Step 3 – Analyze Event Fields

Reviewed the automatically extracted fields associated with the returned events.

Examined information such as:

- host
- source
- sourcetype
- index
- timestamp

Using extracted fields provides additional context and helps identify patterns that may not be immediately visible when reviewing raw events.

### Screenshot

<img width="1143" height="916" alt="image" src="https://github.com/user-attachments/assets/fa4c7605-836a-4c93-a6e6-04ff85760fe2" />


**Caption**

<sub><em>Reviewed extracted fields to gain additional context and better understand the returned events.</em></sub>

---

## Step 4 – Summarize the Results

Applied statistical commands to identify trends within the returned events.

Example:

```spl
index=* author="Splunk" | stats count
```

Summarizing the data helps identify systems generating the most activity and provides a clearer picture of the overall environment.

### Screenshot

<img width="1146" height="339" alt="image" src="https://github.com/user-attachments/assets/d20b7888-2bd2-4359-9ffa-ea6f9d3e991b" />


**Caption**

<sub><em>Summarized the returned events to identify patterns and systems generating the highest levels of activity.</em></sub>

---

## Step 5 – Review the Dashboard

Opened the dashboard created during the previous lab to compare the investigation results with existing visualizations.

Using dashboards provides a quick overview of activity and helps validate observations made during the investigation.

### Screenshot

<img width="1281" height="723" alt="image" src="https://github.com/user-attachments/assets/ab0ee3fb-e687-4d01-b74f-b304ec60c6b3" />


**Caption**

<sub><em>Reviewed dashboard visualizations to compare summarized data and support the investigation.</em></sub>

---

## Step 6 – Review Alerts and Reports

Reviewed the report and alert created during the previous lab to determine whether the investigated activity met any predefined monitoring conditions.

This demonstrates how automated monitoring supports analysts by drawing attention to noteworthy events without requiring constant manual searches.

### Screenshot

<img width="832" height="218" alt="image" src="https://github.com/user-attachments/assets/73fa30d4-bbec-4578-b3b5-febcdbc0b3bb" />


**Caption**

<sub><em>Reviewed previously configured reports and alerts to determine whether the investigated activity met established monitoring conditions.</em></sub>

---

## Step 7 – Document Findings

Reviewed the collected information and documented the overall findings of the investigation.

Based on the available data, determined whether the observed activity appeared consistent with normal system behavior or whether it warranted additional investigation.

Documenting observations is an important part of the incident response process and helps maintain clear records for future analysis.

### Screenshot

<img width="1141" height="321" alt="image" src="https://github.com/user-attachments/assets/67ab202c-5b2a-4025-8ad4-ecf0c414f582" />
<img width="1140" height="646" alt="image" src="https://github.com/user-attachments/assets/6827100f-63c4-450c-add9-b36d28f84c6f" />


**Caption**

<sub><em>Documented the investigation findings after reviewing search results, field data, dashboards, and automated monitoring tools.</em></sub>

## Findings: The reviewed activity was associated with the available Splunk dataset and did not, by itself, provide sufficient evidence of malicious activity. Additional investigation would be warranted if other indicators or anomalous behavior were identified.

---

## What I Learned

This capstone lab brought together the skills developed throughout the Splunk Cloud series into a single investigative workflow. Beginning with a broad search, I progressively narrowed the data using filters, examined extracted fields for additional context, summarized activity with statistical commands, referenced dashboards to visualize trends, and reviewed reports and alerts to support the investigation. Working through these steps reinforced how individual Splunk features complement one another during system monitoring and security analysis.

---

## Skills Learned

- Conducting structured investigations in Splunk Cloud
- Applying SPL to locate relevant events
- Using extracted fields to analyze event data
- Summarizing machine data with statistical commands
- Interpreting dashboards and visualizations
- Leveraging reports and alerts for proactive monitoring
- Documenting investigative findings
- Understanding the workflow of a SOC analyst
