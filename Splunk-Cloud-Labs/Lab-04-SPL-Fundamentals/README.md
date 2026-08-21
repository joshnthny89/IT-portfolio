# 🔍 Lab 04 – SPL Fundamentals

## Objective

Build on previous search techniques by using core Search Processing Language (SPL) commands to organize, filter, and summarize search results. In this lab, I used several foundational SPL commands to investigate machine data more efficiently and present the results in a format that is easier to analyze.

---

## Skills Practiced

- Search Processing Language (SPL)
- Data Organization
- Event Analysis
- Search Optimization
- Log Investigation
- SIEM Fundamentals

---

## Tools Used

- Splunk Cloud Platform
- Search & Reporting App

---

# Lab Walkthrough

## Scenario

During routine monitoring, a large number of events were returned from a search. Rather than manually reviewing every event, the objective was to organize and refine the results using foundational SPL commands. These techniques help analysts quickly identify relevant information while reducing unnecessary data during troubleshooting and security investigations.

---

## Step 1 – Search Indexed Events

Started by performing a broad search to return available events.

```spl
index=*
```

Running a broad search establishes a baseline before applying additional commands to organize and reduce the data.

### Screenshot

<img width="1280" height="911" alt="image" src="https://github.com/user-attachments/assets/741dc68c-a631-4fa1-bced-2cf594c5bae9" />


**Caption**

<sub><em>Performed a broad search to retrieve indexed events before refining the results with SPL commands.</em></sub>

---

## Step 2 – Display Only Relevant Fields

Rather than reviewing every available field, selected only the information needed for analysis.

```spl
index=* | table _time host source sourcetype
```

Displaying only relevant fields makes the search results easier to read and allows important information to stand out.

### Screenshot

<img width="1271" height="910" alt="image" src="https://github.com/user-attachments/assets/ec9bcfe1-b907-4cba-9361-73114d3f7c7c" />


**Caption**

<sub><em>Used the <code>table</code> command to display only the fields most relevant to the investigation.</em></sub>

---

## Step 3 – Sort the Results

Organized the returned events by time.

```spl
index=* | table _time host source | sort -_time
```

Sorting the results places the newest events at the top, making it easier to review recent activity first.

### Screenshot

<img width="1264" height="906" alt="image" src="https://github.com/user-attachments/assets/5751347f-546c-4fa2-9330-df8e9335a33f" />


**Caption**

<sub><em>Sorted the returned events to prioritize reviewing the most recent activity.</em></sub>

---

## Step 4 – Limit the Results

Reduced the number of displayed events.

```spl
index=* | head 20
```

Limiting the output allows analysts to quickly review a manageable sample of data before expanding the search if necessary.

### Screenshot

<img width="1265" height="896" alt="image" src="https://github.com/user-attachments/assets/f748ab1c-9dcc-4e0a-bea8-d7a995bf1048" />
<img width="1761" height="977" alt="image" src="https://github.com/user-attachments/assets/61e71d36-ca29-4b32-b0ea-a891e1eb9f1f" />


**Caption**

<sub><em>Limited the returned events to create a smaller dataset for quicker analysis.</em></sub>

---

## Step 5 – Remove Duplicate Results

Removed duplicate entries to simplify the results.

```spl
index=* | dedup host
```

Removing duplicate values helps identify unique systems without repeatedly displaying identical information.

### Screenshot

<img width="1270" height="787" alt="image" src="https://github.com/user-attachments/assets/69ce69a9-347d-4023-b285-739dffee35cc" />


**Caption**

<sub><em>Removed duplicate hosts to simplify the search results and focus on unique systems.</em></sub>

---

## Step 6 – Combine Multiple Commands

Combined several SPL commands into a single search.

```spl
index=* | table _time host source sourcetype | sort -_time | head 20
```

Using multiple commands together creates a more efficient workflow and demonstrates how simple SPL building blocks can be combined to answer more specific questions.

### Screenshot

<img width="1278" height="910" alt="image" src="https://github.com/user-attachments/assets/df922baa-f923-4acc-aa7b-e5f332199586" />


**Caption**

<sub><em>Combined multiple SPL commands into a single search to organize, sort, and refine the returned events.</em></sub>

---

## What I Learned

This lab introduced the core SPL commands used to organize search results into meaningful information. Rather than manually reviewing every returned event, I learned how commands such as `table`, `sort`, `head`, and `dedup` work together to reduce unnecessary data and make investigations more efficient. These techniques provide the foundation for building more advanced searches throughout the remaining Splunk Cloud labs.

---

## Skills Learned

- Using the `table` command
- Sorting search results
- Limiting returned events
- Removing duplicate values
- Combining SPL commands
- Improving search efficiency
