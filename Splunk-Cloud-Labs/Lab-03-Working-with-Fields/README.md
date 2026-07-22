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

*(Insert screenshot of the Search & Reporting application.)*

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

*(Insert screenshot showing returned events.)*

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

*(Insert screenshot highlighting the Fields panel.)*

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

*(Insert screenshot showing the filtered search.)*

**Caption**

<sub><em>Filtered the returned events using a field value to narrow the search and focus on relevant system activity.</em></sub>

---

## Step 5 – Review Event Details

Expanded one or more events to examine the detailed information contained within them.

Observed how Splunk organizes event data into searchable fields, making it easier to identify important information such as timestamps, hosts, sources, and event-specific details.

### Screenshot

*(Insert screenshot showing an expanded event.)*

**Caption**

<sub><em>Reviewed the detailed event information to better understand how Splunk organizes searchable machine data.</em></sub>

---

## Step 6 – Compare Multiple Field Values

Selected additional field values and observed how each selection refined the search results.

Comparing different fields demonstrates how analysts can quickly isolate events associated with a particular host, source, or data type without manually searching through thousands of log entries.

### Screenshot

*(Insert screenshot showing multiple field selections.)*

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
