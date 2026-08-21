# 🔎 Lab 02 – Searching & Filtering Data

## Objective

Learn how to search and filter indexed machine data within Splunk Cloud using basic Search Processing Language (SPL) commands. This lab introduces the core search functionality used by IT professionals and SOC analysts to quickly locate relevant events, narrow search results, and begin investigating system activity.

---

## Skills Practiced

- Search Processing Language (SPL)
- Event Searching
- Data Filtering
- Time Range Selection
- Log Analysis
- SIEM Fundamentals

---

## Tools Used

- Splunk Cloud Platform
- Search & Reporting App

---

# Lab Walkthrough

## Step 1 – Open the Search & Reporting App

Logged into Splunk Cloud and opened the **Search & Reporting** application. This workspace serves as the primary area for searching indexed machine data, analyzing events, and investigating activity across an environment.

### Screenshot

<img width="2850" height="1494" alt="image" src="https://github.com/user-attachments/assets/d29d1bbc-2210-4b42-8606-05245efaaea2" />


**Caption**

<sub><em>Opened the Search & Reporting application to begin searching and analyzing indexed machine data within Splunk Cloud.</em></sub>

---

## Step 2 – Perform a Basic Search

Entered the following search into the search bar:

```spl
index=*
```

This search returns events from all available indexes and provides an initial view of the data currently stored within Splunk. Running a broad search helps verify that data is being indexed correctly before narrowing the results.

### Screenshot

<img width="1280" height="911" alt="image" src="https://github.com/user-attachments/assets/05a6b719-f816-472e-be87-ab4fc6e8607a" />


**Caption**

<sub><em>Performed a basic search across all indexes to verify available data and become familiar with the search results interface.</em></sub>

---

## Step 3 – Adjust the Time Range

Modified the search time range using the Time Range Picker to display events from a specific period.

Changing the time range is one of the quickest ways to reduce unnecessary results and focus on the timeframe relevant to an investigation or troubleshooting effort.

### Screenshot

<img width="1259" height="603" alt="image" src="https://github.com/user-attachments/assets/46baea00-cc0c-40c2-bc86-f318e412f037" />

<img width="1275" height="908" alt="image" src="https://github.com/user-attachments/assets/6459c53c-60b9-4f20-98ea-c4de5b45bf28" />


**Caption**

<sub><em>Adjusted the search time range to refine the returned events and focus on a specific timeframe.</em></sub>

---

## Step 4 – Filter Search Results

Refined the search by applying additional search criteria to narrow the returned events.

Rather than reviewing every available event, filtering allows analysts to quickly locate information related to a specific host, source, sourcetype, or keyword, making investigations significantly more efficient.

### Screenshot

<img width="1131" height="844" alt="image" src="https://github.com/user-attachments/assets/b1cb1c32-0c7d-4f7e-acd6-51b0d7c0f2d4" />


**Caption**

<sub><em>Applied search filters to narrow the returned events and isolate relevant information for analysis.</em></sub>

---

## Step 5 – Review Returned Events

Examined the returned search results and reviewed the event details displayed by Splunk.

Observed how each event contains valuable information such as timestamps, hosts, sources, and event data that can be used during troubleshooting or security investigations.

### Screenshot

<img width="1273" height="896" alt="image" src="https://github.com/user-attachments/assets/0e21e435-9a60-418d-b7cd-33222acc9f1d" />


**Caption**

<sub><em>Reviewed returned events to better understand how Splunk organizes and presents indexed machine data.</em></sub>

---

## Step 6 – Clear or Modify the Search

Modified or cleared the search query to perform additional searches and observe how different search criteria affect the returned results.

Practicing with simple searches helps build familiarity with SPL and demonstrates how small changes to a query can significantly improve the quality of search results.

### Screenshot
<img width="1140" height="838" alt="image" src="https://github.com/user-attachments/assets/ca6b9783-a40b-45e7-b765-528b722c8f33" />

<img width="1140" height="830" alt="image" src="https://github.com/user-attachments/assets/33f5fbfe-8431-4619-8425-48830b9b98f7" />


**Caption**

<sub><em>Modified the search query to observe how different search criteria impact the returned results.</em></sub>

---

## What I Learned

This lab introduced the fundamentals of searching and filtering data within Splunk Cloud. By performing basic searches, adjusting time ranges, and refining results with additional search criteria, I gained a better understanding of how analysts locate relevant events within large datasets. These foundational search techniques are essential for troubleshooting systems, investigating security events, and building more advanced SPL queries in future labs.

---

## Skills Learned

- Navigating the Search & Reporting application
- Performing basic SPL searches
- Adjusting search time ranges
- Filtering indexed events
- Reviewing event details
- Understanding how Splunk organizes searchable machine data
