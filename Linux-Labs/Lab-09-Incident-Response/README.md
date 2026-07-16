
# 🛡️ Lab 09 - Incident Response

## Overview

In this lab, I simulated the initial triage process of a potential security incident by collecting and reviewing key system information commonly examined during an investigation. Using native macOS command-line tools, I gathered evidence related to the active user, running processes, network activity, system health, and recent log events. This lab combines techniques learned throughout previous labs into a structured incident response workflow.

---

## Skills Demonstrated

- Incident Response
- Initial System Triage
- Evidence Collection
- Process Enumeration
- Network Analysis
- System Health Verification
- Log Investigation
- Linux/macOS Command Line

---

## Tools Used

- macOS Terminal
- Bash
- `date`
- `whoami`
- `ps`
- `netstat`
- `df`
- `who`
- `tail`

---

# Investigation Scenario

A user reported that their workstation was behaving unusually after installing new software. As the responding analyst, the objective was to perform an initial triage by gathering system information that could assist in identifying suspicious activity while documenting the system's current state.

---

# Investigation Workflow

---

## Step 1 – Establish the Investigation Context

The investigation began by documenting the current date and identifying the active user account. Recording this information establishes the investigation timeline and identifies the user context associated with the system.

### Commands Used

```bash
date
whoami
```

### Screenshot

![Step 1](screenshots/step1.png)

<sub><em>Established the investigation timeline and identified the active user account before collecting additional system information.</em></sub>

---

## Step 2 – Review Running Processes

Reviewed the currently running processes to establish a baseline of active applications and services. This information helps identify unexpected or suspicious processes during an investigation.

### Command Used

```bash
ps aux | head
```

### Screenshot

![Step 2](screenshots/step2.png)

<sub><em>Reviewed active processes to establish a baseline of running applications and services during the initial investigation.</em></sub>

---

## Step 3 – Review Active Network Connections

Examined active network connections and listening ports to identify current communication occurring on the system.

### Command Used

```bash
netstat -an | head
```

### Screenshot

![Step 3](screenshots/step3.png)

<sub><em>Reviewed active network connections to identify listening services and current network activity.</em></sub>

---

## Step 4 – Verify Filesystem Health

Checked filesystem utilization to verify sufficient available disk space and identify any storage conditions that could impact logging or system performance.

### Command Used

```bash
df -h
```

### Screenshot

![Step 4](screenshots/step4.png)

<sub><em>Verified filesystem utilization as part of assessing overall system health during the investigation.</em></sub>

---

## Step 5 – Review Active User Sessions

Reviewed currently logged-in users to determine which user sessions were active at the time of the investigation.

### Command Used

```bash
who
```

### Screenshot

![Step 5](screenshots/step5.png)

<sub><em>Reviewed active user sessions to identify users currently logged into the system.</em></sub>

---

## Step 6 – Review Recent System Log Activity

Examined the most recent system log entries to identify any events that could assist in understanding recent system activity.

### Command Used

```bash
tail /private/var/log/keybagd.log.0
```

### Screenshot

![Step 6](screenshots/step6.png)

<sub><em>Reviewed recent system log entries to identify events that may require additional investigation.</em></sub>

---

## Investigation Summary

The investigation followed a structured triage workflow by documenting the current user, reviewing active processes, examining network connections, verifying system health, identifying active user sessions, and reviewing recent system log activity. While no specific indicators of compromise were identified during this simulated investigation, the workflow demonstrates a repeatable methodology commonly used during the early stages of incident response.

---

## Skills Learned

- Conducting an initial incident response triage
- Collecting and documenting system evidence
- Reviewing active processes
- Investigating network activity
- Assessing system health
- Reviewing system logs
- Applying a structured investigation methodology
