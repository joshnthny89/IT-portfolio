# 🤖 Lab 10 – Basic Bash Automation

## Objective

Learn how a simple Bash script can automate common system information gathering tasks. Instead of manually entering several commands one at a time, a script allows multiple commands to be executed in sequence, improving efficiency and consistency during troubleshooting and incident response.

---

## Skills Practiced

- Bash scripting fundamentals
- Basic automation
- System information collection
- Process enumeration
- Network connection review
- Disk usage analysis
- Log collection
- Incident response preparation

---

## Commands Used

```bash
#!/bin/bash

echo "===== Date ====="
date

echo "===== Current User ====="
whoami

echo "===== Running Processes ====="
ps aux | head

echo "===== Network Connections ====="
netstat -an | head

echo "===== Disk Usage ====="
df -h

echo "===== Logged In Users ====="
who

echo "===== Recent Log Entries ====="
tail /private/var/logs/keybagd.log.0
```

---

# Lab Walkthrough

## Step 1 – Create the Bash Script

Create a new script named `system_info.sh` using a text editor.

Example:

```bash
nano system_info.sh
```

Paste the script contents into the file and save it.

### Screenshot

<img width="850" height="42" alt="image" src="https://github.com/user-attachments/assets/8eaf264d-0c8e-4714-9477-9eeae2ba2bb7" />

<img width="799" height="656" alt="image" src="https://github.com/user-attachments/assets/31c69e77-f454-409b-b5f2-f037f87cc69d" />


**Caption**

<sub><em>Created a Bash script to automate the collection of common system information used during troubleshooting and incident response.</em></sub>

---

## Step 2 – Make the Script Executable

Before a script can be run directly, it must be given execute permissions.

Command:

```bash
chmod +x system_info.sh
```

Verify the permission change:

```bash
ls -l system_info.sh
```

### Screenshot

<img width="1010" height="92" alt="image" src="https://github.com/user-attachments/assets/d756ad4c-8dbd-4232-b79b-99c3340b7ec4" />


**Caption**

<sub><em>Granted execute permissions to the Bash script using <code>chmod +x</code>, allowing it to be run as a program.</em></sub>

---

## Step 3 – Execute the Script and Review the Output

Run the script from the current directory.

Command:

```bash
./system_info.sh
```

The script automatically gathers several pieces of useful system information:

- Current date and time
- Current user
- Running processes
- Active network connections
- Disk usage
- Logged-in users
- Recent system log entries

Review each section of the output and observe how the script organizes the information using descriptive headings. This makes the results much easier to interpret than running each command individually and demonstrates how even a simple Bash script can improve efficiency during troubleshooting and incident response.

### Screenshot

<img width="1712" height="1314" alt="image" src="https://github.com/user-attachments/assets/75d55ae5-d712-4cc8-a590-d858368a58b2" />
<img width="1720" height="666" alt="image" src="https://github.com/user-attachments/assets/b960bc89-b0d2-4b22-9a24-dbeee3893d02" />


**Caption**

<sub><em>Executed the Bash automation script to collect and organize system information into clearly labeled sections, demonstrating how automation improves consistency and efficiency during basic system triage.</em></sub>


---

## Step 5 – Understanding the Script

This automation demonstrates several important Bash scripting concepts:

- Sequential command execution
- Using `echo` to create readable output
- Combining multiple administrative commands into one workflow
- Automating repetitive tasks

Although simple, this approach scales well as additional commands are added to support troubleshooting, incident response, or security monitoring.

---

## What I Learned

This lab introduced the fundamentals of Bash automation by combining multiple Linux/macOS commands into a single executable script. Automating repetitive tasks reduces manual effort, minimizes the chance of missing important information, and creates a repeatable process for gathering system data during troubleshooting or security investigations.
