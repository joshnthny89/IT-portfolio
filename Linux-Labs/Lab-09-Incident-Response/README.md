
# 🛡️ Lab 09 - Incident Response

## Overview

In this lab, I simulated the initial triage process of a security incident by collecting key system information commonly reviewed during an investigation. The objective was to gather evidence, establish a system baseline, and identify indicators that may warrant further investigation.

---

## Skills Demonstrated

- Incident Response
- Initial System Triage
- Evidence Collection
- Linux Administration
- Process Enumeration
- Network Investigation
- Log Collection

---

## Tools Used

- macOS Terminal
- date
- whoami
- ps
- netstat
- df
- who
- tail

---

# Investigation Workflow

---

## Step 1 – Identify Investigation Context

Collected the current date and active user.

### Commands Used

```bash
date
whoami
```

### Screenshot

![Step 1](screenshots/step1.png)

<sub><em>Established the investigation timeframe and identified the active user context.</em></sub>

---

## Step 2 – Review Running Processes

Reviewed currently running processes.

### Command Used

```bash
ps aux | head
```

### Screenshot

![Step 2](screenshots/step2.png)

<sub><em>Collected process information to identify active applications and services.</em></sub>

---

## Step 3 – Examine Network Activity

Reviewed current network connections.

### Command Used

```bash
netstat -an | head
```

### Screenshot

![Step 3](screenshots/step3.png)

<sub><em>Reviewed active network connections and listening ports as part of the initial system triage.</em></sub>

---

## Step 4 – Verify System Resources

Checked filesystem utilization.

### Command Used

```bash
df -h
```

### Screenshot

![Step 4](screenshots/step4.png)

<sub><em>Verified available disk space to identify potential storage issues that could impact system operation or logging.</em></sub>

---

## Step 5 – Review Active Users

Verified active user sessions.

### Command Used

```bash
who
```

### Screenshot

![Step 5](screenshots/step5.png)

<sub><em>Reviewed active user sessions to identify users currently logged into the system.</em></sub>

---

## Step 6 – Collect Recent Log Activity

Reviewed recent system log entries.

### Command Used

```bash
tail /private/var/log/keybagd.log.0
```

### Screenshot

![Step 6](screenshots/step6.png)

<sub><em>Collected recent log activity to identify system events and potential indicators requiring further investigation.</em></sub>

---

## Skills Learned

- Performing initial incident response triage
- Gathering system evidence
- Reviewing processes and network activity
- Collecting log data
- Building a structured investigation workflow
