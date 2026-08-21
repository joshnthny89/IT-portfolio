# ☁️ Lab 01 – Splunk Cloud Introduction

## Objective

Become familiar with the Splunk Cloud Platform by exploring the user interface, identifying the primary navigation menus, and understanding how Splunk organizes machine data for searching, monitoring, and security investigations. This lab establishes the foundation for future labs involving Search Processing Language (SPL), dashboards, alerts, and incident investigations, incorporating core SIEM architectural principles like schema-on-read and metadata field indexing.

---

## Skills Practiced

- Splunk Cloud Navigation
- SIEM Fundamentals & Tenant Architecture
- Security Monitoring & Log Management
- Data Exploration & Schema-on-Read
- Splunk User Interface (Search & Reporting)
- Metadata & Extracted Field Analysis
- Log Management


---

## Tools Used

- Splunk Cloud Platform (SaaS Tenant)
- Web Browser

---

# Lab Walkthrough

## Step 1 – Log in to Splunk Cloud

Logged into the Splunk Cloud Platform using an authorized user account.

After authentication against the secure tenant URL, session initialization was governed by Role-Based Access Control (RBAC). The Splunk Cloud home dashboard was then displayed, providing centralized access to the Search & Reporting application, management panels, and global navigation controls.

### Screenshot

<img width="1830" height="634" alt="image" src="https://github.com/user-attachments/assets/1a802a56-05f5-465d-b09e-4bb4edeba90a" />
<img width="2878" height="1572" alt="image" src="https://github.com/user-attachments/assets/0531bf3e-d88b-4227-8dff-388e9cee61d8" />


**Caption**

<sub><em>Logged into the Splunk Cloud Platform and accessed the main dashboard.</em></sub>

---

## Step 2 – Explore the Splunk Home Dashboard

Reviewed the main Splunk dashboard and identified commonly used navigation areas including:

- Search & Reporting
- Apps
- Dashboards
- Activity 
- Settings 
- Help

Understanding the dashboard layout provides the foundation for navigating Splunk efficiently during future investigations.

### Screenshot

<img width="2850" height="1494" alt="image" src="https://github.com/user-attachments/assets/7893b8a7-fb50-4bdd-83f7-74c78542eea3" />
<img width="2856" height="1462" alt="image" src="https://github.com/user-attachments/assets/e5dabcd2-8cc8-4844-bfb8-1882115a8227" />
<img width="2866" height="1416" alt="image" src="https://github.com/user-attachments/assets/f6293c26-f3aa-425f-a6f4-ec9b36e5c980" />
<img width="1392" height="1186" alt="image" src="https://github.com/user-attachments/assets/daa61fea-a28e-44d6-8d5d-18de5c6d3b4a" />
<img width="1434" height="764" alt="image" src="https://github.com/user-attachments/assets/5a683c91-6224-490d-a841-5734f6368937" />


**Caption**

<sub><em>Explored the Splunk Cloud dashboard to become familiar with the primary navigation menus and available applications.</em></sub>

---

## Step 3 – Open the Search & Reporting App

Navigated to the **Search & Reporting** application.

This application serves as the primary workspace for searching indexed data, building SPL queries, analyzing events, and performing security investigations.

### Screenshot

<img width="2850" height="1494" alt="image" src="https://github.com/user-attachments/assets/e883bd8f-80f4-4337-a913-fa1293c8dbb0" />


**Caption**

<sub><em>Opened the Search & Reporting application, the primary workspace for querying and analyzing indexed data.</em></sub>

---

## Step 4 – Explore the Search Interface

Reviewed the Search & Reporting interface and identified its major components, including:

- Search Bar
- Time Range Picker
- Event Viewer
- Fields Sidebar
- Search Controls

These tools are used throughout the remaining Splunk labs.

### Screenshot

<img width="2864" height="1492" alt="image" src="https://github.com/user-attachments/assets/abfa6a2c-efac-48e7-afb3-1bc14ef9b820" />

**Caption**

<sub><em>Reviewed the Search & Reporting interface and identified the tools used to search and analyze machine data.</em></sub>

---

## Step 5 – Review Indexed Data

Verified that indexed data was available for searching by examining the Events pane and available fields.

Observed how Splunk organizes machine data into searchable events that can later be filtered, analyzed, and visualized.

### Screenshot

<img width="2870" height="1558" alt="image" src="https://github.com/user-attachments/assets/90a8c33d-71ff-42c1-994a-85371610f285" />


**Caption**

<sub><em>Reviewed indexed events to understand how Splunk stores and displays searchable machine data.</em></sub>

---

## Step 6 – Explore Available Fields

Examined the Fields sidebar to observe how Splunk automatically extracts searchable information from indexed events.

Examples of commonly extracted fields include:

- host
- source
- sourcetype
- index
- timestamp

Understanding these fields is essential for building effective SPL searches and filtering results.

### Screenshot

<img width="2374" height="1332" alt="image" src="https://github.com/user-attachments/assets/59574662-6346-42bd-b56b-a4bec47fcbf1" />
<img width="2586" height="1238" alt="image" src="https://github.com/user-attachments/assets/7f618219-a781-4340-95f5-5807fb68816b" />
<img width="2546" height="1298" alt="image" src="https://github.com/user-attachments/assets/08a0e1f1-f681-4ff4-8521-aa62407a03ef" />


**Caption**

<sub><em>Explored automatically extracted fields used to filter, organize, and investigate machine data.</em></sub>

---

## What I Learned

This lab introduced the Splunk Cloud Platform and its primary interface. By exploring the Search & Reporting application, navigation menus, indexed events, and extracted fields, I developed a foundational understanding of how Splunk organizes and presents machine data. This knowledge provides the basis for future labs involving SPL searches, dashboards, alerts, and security investigations.

---

## Skills Learned

- Navigating the Splunk Cloud Platform
- Understanding SIEM fundamentals
- Exploring the Search & Reporting application
- Identifying indexed data
- Understanding extracted fields
- Becoming familiar with the Splunk interface

