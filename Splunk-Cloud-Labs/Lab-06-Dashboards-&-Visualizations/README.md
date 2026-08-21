# 📈 Lab 06 – Dashboards & Visualizations

## Objective

Learn how to transform search results into visual dashboards that make large amounts of machine data easier to understand and monitor. This lab demonstrates how charts, graphs, and dashboard panels can quickly highlight trends, making it easier to identify patterns, monitor system activity, and support security investigations.

---

## Skills Practiced

- Dashboard Creation
- Data Visualization
- Search Processing Language (SPL)
- Statistical Analysis
- SIEM Monitoring
- Security Reporting

---

## Tools Used

- Splunk Cloud Platform
- Search & Reporting App
- Dashboards

---

# Lab Walkthrough

## Scenario

After using statistical commands to summarize machine data, the next step is presenting that information in a format that can be monitored at a glance. Dashboards provide analysts with a centralized view of system activity, allowing important trends and metrics to be identified without running individual searches repeatedly.

---

## Step 1 – Perform a Statistical Search

Started by running a statistical search that summarized indexed events.

Example:

```spl
index=* | stats count by author
```

This search provides a dataset that can be converted into a visualization.

### Screenshot

<img width="1280" height="712" alt="image" src="https://github.com/user-attachments/assets/dfb45a20-8f99-4cfd-a997-0500e4fa4eb1" />


**Caption**

<sub><em>Performed a statistical search to summarize indexed events before creating a dashboard visualization.</em></sub>

---

## Step 2 – Create a Visualization

Selected the **Visualization** tab within the Search & Reporting application to convert the search results into a graphical format.

Splunk automatically generated several visualization options including:

- Bar Chart
- Column Chart
- Pie Chart
- Line Chart
- Area Chart

### Screenshot

<img width="1282" height="832" alt="image" src="https://github.com/user-attachments/assets/488bf24a-8425-4f2d-85ed-1b1996f4794a" />


**Caption**

<sub><em>Converted the search results into a visualization to better identify trends within the data.</em></sub>

---

## Step 3 – Explore Different Chart Types

Viewed the same search results using multiple visualization types.

Comparing different chart styles demonstrates how each one presents information differently depending on the type of data being analyzed.

### Screenshot
<img width="1129" height="744" alt="image" src="https://github.com/user-attachments/assets/fcbf9e58-de8e-4878-a9fa-4486f20eb1ee" />
<img width="1137" height="747" alt="image" src="https://github.com/user-attachments/assets/9a2f1b5b-23ad-4628-8921-8d680ae4be40" />
<img width="1143" height="738" alt="image" src="https://github.com/user-attachments/assets/633266c0-d450-4ebe-a182-1f536a6bbe0b" />


**Caption**

<sub><em>Compared multiple chart types to determine which visualization best represented the search results.</em></sub>

---

## Step 4 – Save the Visualization to a Dashboard

Saved the completed visualization to a new dashboard.

Provided the dashboard with a descriptive title and organized the visualization for future monitoring.

### Screenshot

<img width="1265" height="760" alt="image" src="https://github.com/user-attachments/assets/219e26fd-8ea1-451b-ac30-b55b48b3df7f" />


**Caption**

<sub><em>Saved the visualization to a dashboard, creating a reusable view for monitoring summarized system activity.</em></sub>

---

## Step 5 – Review the Dashboard

Opened the completed dashboard and reviewed the visualization.

Verified that the dashboard displayed the expected data and provided an easy-to-read summary of system activity without rerunning the original search.

### Screenshot

<img width="1142" height="372" alt="image" src="https://github.com/user-attachments/assets/8f025845-94f1-4d2e-8c20-c218e1fb8b44" />


**Caption**

<sub><em>Reviewed the completed dashboard to verify that it accurately displayed the summarized search results.</em></sub>

---

## Step 6 – Update the Dashboard

Modified the dashboard by adjusting the panel layout, title, or visualization settings.

Making small adjustments improves readability and allows dashboards to be customized for different monitoring requirements.

### Screenshot
<img width="1139" height="650" alt="image" src="https://github.com/user-attachments/assets/3a58ff60-35d9-4ef8-a038-e9b005ca26a9" />

<img width="1278" height="730" alt="image" src="https://github.com/user-attachments/assets/481e98b7-ee72-4e95-8a10-61d1ce5946c9" />


**Caption**

<sub><em>Updated the dashboard layout and visualization settings to improve readability and usability.</em></sub>

---

## What I Learned

This lab demonstrated how Splunk dashboards transform search results into visual representations that are easier to interpret and monitor. By converting statistical data into charts and organizing those visualizations within a dashboard, I gained a better understanding of how analysts monitor system activity, identify trends, and quickly recognize changes that may require further investigation. Dashboards provide a centralized view of important information, reducing the need to repeatedly perform the same searches.

---

## Skills Learned

- Creating Splunk visualizations
- Comparing chart types
- Building dashboards
- Saving searches as dashboard panels
- Organizing dashboard layouts
- Presenting machine data visually
- Supporting system monitoring through dashboards
