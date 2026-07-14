# Lab 08 - Log Searching

## Objective

The objective of this lab is to demonstrate how command-line tools can be used to efficiently search, filter, and analyze system log files. Rather than manually reviewing thousands of log entries, administrators and security analysts use commands such as `grep`, `wc`, `sort`, `uniq`, and `cut` to locate relevant events, identify recurring patterns, and quickly extract useful information during troubleshooting and incident response.

---

## Skills Demonstrated

- Searching log files using `grep`
- Performing case-insensitive searches
- Counting matching log entries
- Identifying repeated events
- Sorting command output
- Filtering duplicate results
- Extracting specific fields from log entries
- Using command pipelines
- Basic log analysis techniques
- Linux/macOS command-line proficiency

---

# Step 1 - Navigate to the Logs Directory

```bash
cd /private/var/log
pwd
```

Verified the current working directory and navigated to the macOS system log directory where log files are stored.

### Screenshot

<img width="427" height="49" alt="image" src="https://github.com/user-attachments/assets/872cbac7-2386-4640-9471-18eadbac25f2" />

<sub><em>Navigated to the macOS system log directory and verified the current working directory before performing log searches.</em></sub>

---

# Step 2 - Search for Failed Events

```bash
grep -i "failed" keybagd.log.3
```

Performed a case-insensitive search to locate entries containing the keyword **failed**.

### Screenshot

<img width="860" height="654" alt="image" src="https://github.com/user-attachments/assets/553a41b3-0938-4dd4-9f51-6dec750e194e" />

<sub><em>Used the <code>grep</code> command to quickly locate failed events within the selected log file.</em></sub>

---

# Step 3 - Count Matching Entries

```bash
grep -i "failed" keybagd.log.3 | wc -l
```

Counted the total number of log entries containing the keyword **failed**.

### Screenshot

<img width="576" height="33" alt="image" src="https://github.com/user-attachments/assets/be70ae56-f9cb-453c-b7f7-d6ab604806b1" />

<sub><em>Piped the output of <code>grep</code> into <code>wc -l</code> to determine the number of matching log entries.</em></sub>

---

# Step 4 - Find Unique Error Messages

```bash
grep -i "failed" keybagd.log.3 | sort | uniq
```

Sorted the search results and removed duplicate entries to identify unique log events.

### Screenshot

*(Insert Screenshot Here)*

<sub><em>Sorted the search results and removed duplicate entries to identify unique failed events.</em></sub>

---

# Step 5 - Search for Errors

```bash
grep -i "error" keybagd.log.3
```

Searched the log file for entries containing the keyword **error**.

### Screenshot

*(Insert Screenshot Here)*

<sub><em>Performed a case-insensitive search for log entries containing the keyword <code>error</code>.</em></sub>

---

# Step 6 - Display the Most Recent Matching Events

```bash
grep -i "error" keybagd.log.3 | tail
```

Displayed the last several matching log entries to review the most recent events.

### Screenshot

*(Insert Screenshot Here)*

<sub><em>Combined <code>grep</code> with <code>tail</code> to display the most recent matching log entries.</em></sub>

---

# Step 7 - Extract Relevant Information

```bash
grep -i "error" keybagd.log.3 | cut -d' ' -f1-6
```

Extracted the first six fields from each matching log entry to simplify the output and focus on the timestamp and event information.

### Screenshot

*(Insert Screenshot Here)*

<sub><em>Used the <code>cut</code> command to extract specific fields from matching log entries, making the output easier to analyze.</em></sub>

---

## What I Learned

Throughout this lab, I practiced searching and filtering system log files using common command-line utilities. Rather than manually reviewing large amounts of log data, I used command pipelines to locate specific events, count occurrences, remove duplicate entries, and simplify output for analysis. These techniques improve efficiency during troubleshooting and incident response by allowing analysts to quickly focus on relevant information within large datasets.

---

## Analyst Observation

Searching and filtering log files is a fundamental skill used by system administrators and Security Operations Center (SOC) analysts. Commands such as `grep`, `sort`, `uniq`, `wc`, `cut`, and `tail` allow large volumes of log data to be reduced into meaningful information, making it easier to identify recurring events, investigate errors, and establish timelines during security investigations.
