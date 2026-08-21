# 🏷️ Lab 03 – Working with Fields

## Objective

Learn how Splunk automatically extracts fields from indexed events and how those fields can be used to organize, filter, and investigate data more efficiently. This lab builds on the previous search exercises by introducing field-based analysis, allowing searches to become more targeted and meaningful.

---

## Skills Practiced

- Field Exploration
- Field Filtering
- Event Analysis
- Search Processing Language (SPL)
- Data Organization
- SIEM Fundamentals

---

## Tools Used

- Splunk Cloud Platform
- Search & Reporting App

---

# Lab Walkthrough

## Step 1 – Open the Search & Reporting App

Logged into Splunk Cloud and navigated to the **Search & Reporting** application. This workspace provides access to indexed events and the fields automatically extracted from those events.

### Screenshot

<img width="2850" height="1494" alt="image" src="https://github.com/user-attachments/assets/bd96a8ba-a020-4ffe-90ab-39cc333c30b6" />


**Caption**

<sub><em>Opened the Search & Reporting application to begin exploring indexed events and their associated fields.</em></sub>

---

## Step 2 – Run a Search to Generate Events

Performed a basic search to return indexed events.

```spl
index=*
```

Returning a collection of events allows Splunk to display the available fields that can be used to further refine searches and investigate specific data.

### Screenshot

<img width="1275" height="908" alt="image" src="https://github.com/user-attachments/assets/7014f5db-b5e0-4a59-92e3-302f023fa629" />


**Caption**

<sub><em>Executed a search to return indexed events and display the automatically extracted fields available for analysis.</em></sub>

---

## Step 3 – Explore the Fields Sidebar

Reviewed the **Fields** panel located on the left side of the Search & Reporting interface.

Observed commonly extracted fields including:

- host
- source
- sourcetype
- index

Splunk automatically identifies and organizes these fields, making it easier to locate and analyze specific information without manually reviewing every event.

### Screenshot

<img width="1277" height="884" alt="image" src="https://github.com/user-attachments/assets/d46aa9e9-e738-42ef-8dd6-c517e9c9639d" />


**Caption**

<sub><em>Explored the Fields sidebar to identify the metadata automatically extracted from indexed events.</em></sub>

---

## Step 4 – Filter Events Using a Field

Selected one of the available fields and filtered the search results using one of its values.

For example:

```spl
index=* host="<hostname>"
```

or by simply selecting a field value directly from the Fields panel.

Filtering by field values significantly reduces the number of returned events, helping analysts focus on the information most relevant to an investigation.

### Screenshot

<img width="1278" height="906" alt="image" src="https://github.com/user-attachments/assets/f4a3e1b8-c105-4d8f-963c-ff4e08229652" />


**Caption**

<sub><em>Filtered the returned events using a field value to narrow the search and focus on relevant system activity.</em></sub>

---

## Step 5 – Review Event Details

Expanded one or more events to examine the detailed information contained within them.

Observed how Splunk organizes event data into searchable fields, making it easier to identify important information such as timestamps, hosts, sources, and event-specific details.

### Screenshot

<img width="1279" height="905" alt="image" src="https://github.com/user-attachments/assets/5024e544-013f-4ebc-993b-bc10d0352c6e" />
<img width="1124" height="895" alt="image" src="https://github.com/user-attachments/assets/56d4297a-9873-4b67-84f0-042d5f10d9d0" />


**Caption**

<sub><em>Reviewed the detailed event information to better understand how Splunk organizes searchable machine data.</em></sub>

---

## Step 6 – Compare Multiple Field Values

Selected additional field values and observed how each selection refined the search results.

Comparing different fields demonstrates how analysts can quickly isolate events associated with a particular host, source, or data type without manually searching through thousands of log entries.

### Screenshot

<img width="1287" height="913" alt="image" src="https://github.com/user-attachments/assets/3c7a259c-8192-4039-9c6c-02781edca178" />
<img width="1274" height="918" alt="image" src="https://github.com/user-attachments/assets/aec34e52-ed8e-430e-be64-f2ca4285683e" />


**Caption**

<sub><em>Compared multiple field values to further refine the search results and isolate relevant events.</em></sub>

---

## What I Learned

This lab introduced one of Splunk's most powerful features: automatically extracted fields. Rather than manually reviewing every event, I learned how fields can be used to quickly organize, filter, and investigate machine data. By selecting and comparing field values, I was able to narrow search results and focus on the events most relevant to the task at hand. These techniques form the foundation for more advanced searches and security investigations performed by SOC analysts.

---

## Skills Learned

- Understanding extracted fields
- Filtering searches using field values
- Reviewing event details
- Navigating the Fields sidebar
- Organizing indexed machine data
- Improving search efficiency through field-based analysis
