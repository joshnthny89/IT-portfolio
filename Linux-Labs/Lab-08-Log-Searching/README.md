# 🔍 Lab 08 - Log Searching

## Overview

In this lab, I expanded on the previous log analysis exercises by using command-line tools to efficiently search, filter, and extract information from system log files. These techniques allow administrators and security analysts to quickly locate relevant events without manually reviewing large amounts of log data.

---

## Skills Demonstrated

- Log Searching
- Pattern Matching
- Event Filtering
- Command Pipelines
- Linux Command Line
- Security Investigation
- Troubleshooting

---

## Tools Used

- macOS Terminal
- grep
- wc
- sort
- uniq
- cut

---

# Search Workflow

---

## Step 1 – Search for Failed Events

Performed a case-insensitive search to locate log entries containing the keyword **failed**.

### Command Used

```bash
grep -i "failed" keybagd.log.3
```

### Screenshot

<img width="860" height="654" alt="image" src="https://github.com/user-attachments/assets/553a41b3-0938-4dd4-9f51-6dec750e194e" />

<sub><em>Used <code>grep -i</code> to locate log entries containing the keyword <code>failed</code>, demonstrating a common technique for identifying errors during troubleshooting and security investigations.</em></sub>

---

## Step 2 – Count Matching Events

Counted the total number of matching log entries.

### Command Used

```bash
grep -i "failed" keybagd.log.3 | wc -l
```

### Screenshot

<img width="576" height="33" alt="image" src="https://github.com/user-attachments/assets/be70ae56-f9cb-453c-b7f7-d6ab604806b1" />


<sub><em>Combined <code>grep</code> with <code>wc -l</code> to quickly determine how many matching events were present within the log file.</em></sub>

---

## Step 3 – Identify Unique Results

Sorted the search results and removed duplicate entries.

### Command Used

```bash
grep -i "failed" keybagd.log.3 | sort | uniq
```

### Screenshot

<img width="853" height="652" alt="image" src="https://github.com/user-attachments/assets/79b6fced-7c9d-4297-984b-d635a05e11fc" />


<sub><em>Used a command pipeline to sort search results and remove duplicate entries, making recurring events easier to identify.</em></sub>

---

## Step 4 – Search for Multiple Event Types

Searched for multiple keywords simultaneously.

### Command Used

```bash
grep -Ei "failed|error" keybagd.log.3
```

### Screenshot

<img width="856" height="653" alt="image" src="https://github.com/user-attachments/assets/23250af4-e5a4-4f30-bd53-dcfd7aeabb6f" />

<sub><em>Used an extended regular expression to search for multiple event types in a single command.</em></sub>

---

## Step 5 – Extract Relevant Fields

Reduced the output to display only the first six fields from each matching log entry.

### Command Used

```bash
grep -i "failed" keybagd.log.3 | cut -d' ' -f1-6
```

### Screenshot

<img width="641" height="655" alt="image" src="https://github.com/user-attachments/assets/c7160d16-b068-466b-81cd-117631367572" />

<sub><em>Used the <code>cut</code> command to extract selected fields from matching log entries, simplifying the output for analysis.</em></sub>

---

## Step 6 – Save Search Results for Further Analysis

Redirected the matching log entries into a text file stored within my CyberLabs workspace for future review and documentation.

### Command Used

```bash
grep -i "failed" /private/var/logs/keybagd.1og.3 >failed_events.txt
cat ~/CyberLabs/failed_events.txt
```

### Screenshot

<img width="853" height="305" alt="image" src="https://github.com/user-attachments/assets/3809700f-4096-42e1-86cb-15b7031d8f65" />



<sub><em>Redirected matching log entries into <code>failed_events.txt</code> within my CyberLabs workspace, demonstrating how investigation results can be preserved for documentation and additional analysis. Then verified the contents of <code>failed_events.txt</code> with the <code>cat</code> command to ensure the filtered log entries were successfully exported and available for further investigation.</em></sub>

---

## Skills Learned

- Searching system logs using keywords
- Filtering events with `grep`
- Counting matching log entries
- Using command pipelines to refine results
- Extracting relevant data from log files
- Redirecting command output to a file
- Preserving investigation evidence for future analysis
- Verifying exported log data
