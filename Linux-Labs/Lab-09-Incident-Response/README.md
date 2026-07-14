# Lab 09 - Incident Response

## Objective

The objective of this lab is to demonstrate the initial steps of a basic incident response investigation using native macOS command-line tools. During an investigation, security analysts collect information about the current user, running processes, active network connections, and recent system activity to establish a baseline and identify potential indicators of compromise.

---

## Skills Demonstrated

- System information gathering
- User identification
- Process enumeration
- Network connection analysis
- Log searching
- Evidence collection
- Basic incident response workflow
- Linux/macOS command-line proficiency

---

# Step 1 - Identify the Current User

```bash
whoami
id
```

Identified the currently logged-in user account and displayed the associated user ID (UID), group ID (GID), and group memberships. This information establishes which account is performing the investigation.

### Screenshot

*(Insert Screenshot Here)*

<sub><em>Verified the current user account and associated security identifiers using the <code>whoami</code> and <code>id</code> commands.</em></sub>

---

# Step 2 - Identify Running Processes

```bash
ps aux
```

Displayed all active processes running on the system to establish a baseline of current system activity.

### Screenshot

*(Insert Screenshot Here)*

<sub><em>Enumerated active system processes using the <code>ps aux</code> command to establish a baseline of running applications and services.</em></sub>

---

# Step 3 - Review Active Network Connections

```bash
netstat -an
```

Displayed active network connections and listening ports to identify current network activity.

### Screenshot

*(Insert Screenshot Here)*

<sub><em>Reviewed active network connections and listening ports using the <code>netstat -an</code> command.</em></sub>

---

# Step 4 - Review Recent Log Entries

```bash
tail keybagd.log.0
```

Displayed the most recent entries within the selected log file to identify recent system events.

### Screenshot

*(Insert Screenshot Here)*

<sub><em>Reviewed the most recent system log entries using the <code>tail</code> command.</em></sub>

---

# Step 5 - Search for Failed Events

```bash
grep -i "failed" keybagd.log.0
```

Performed a case-insensitive search to locate log entries containing the keyword **failed**, allowing potentially significant events to be identified quickly.

### Screenshot

*(Insert Screenshot Here)*

<sub><em>Searched the log file for failed events using the <code>grep</code> command to identify potential issues requiring further investigation.</em></sub>

---

# Step 6 - Count Failed Events

```bash
grep -i "failed" keybagd.log.0 | wc -l
```

Counted the number of matching log entries to quantify the frequency of failed events.

### Screenshot

*(Insert Screenshot Here)*

<sub><em>Counted matching failed events using a command pipeline to quickly measure the occurrence of specific log entries.</em></sub>

---

# Step 7 - Identify Network Configuration

```bash
ifconfig
```

Displayed network interface information to verify the system's current network configuration.

### Screenshot

*(Insert Screenshot Here)*

<sub><em>Reviewed network interface configuration using the <code>ifconfig</code> command as part of the evidence collection process.</em></sub>

---

# Step 8 - Collect Evidence Summary

```bash
date
hostname
pwd
```

Collected the current date, hostname, and working directory to document basic environmental information during the investigation.

### Screenshot

*(Insert Screenshot Here)*

<sub><em>Collected basic system information to document the investigation environment.</em></sub>

---

## What I Learned

This lab demonstrated the initial stages of an incident response investigation by collecting information about the current user, running processes, network activity, and recent system events. Rather than focusing on a single command, the lab emphasized gathering multiple sources of information to establish a baseline and identify activity that may warrant further analysis.

---

## Analyst Observation

During an incident response investigation, analysts begin by collecting volatile system information before it changes. Reviewing active processes, network connections, system logs, and user information helps establish a timeline of events and provides valuable context for identifying suspicious activity. Using built-in command-line tools enables analysts to rapidly gather evidence while minimizing changes to the affected system.
