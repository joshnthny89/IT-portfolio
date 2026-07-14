# Lab 07 - Log Analysis

## Objective

Learn how to locate, inspect, and analyze Linux system log files using command-line tools. This lab focuses on reviewing system activity, understanding log file structure, and developing foundational skills used in system administration and cybersecurity investigations.

---

## Skills Demonstrated

- Linux log file navigation
- System log analysis
- Viewing log files with command-line tools
- Reading large files efficiently
- Command piping
- Basic troubleshooting
- Security log review

---

## Tools Used

- macOS Terminal
- Linux Command Line

---

## Commands Used

```bash
cd /var/log
pwd
ls
ls -lh
head install.log
tail install.log
less install.log
cat install.log | head -20
grep -i "failed" keybagd.log.3
```

> **Note:** If `install.log` is unavailable, another available log file within `/var/log` may be substituted.

---

# Step 1 - Navigate to the Log Directory

```bash
cd /var/log
pwd
```

Navigated to the system log directory and verified the current working directory. Most Linux and Unix-based operating systems store important system log files within this location.

### Screenshot

<img width="418" height="99" alt="image" src="https://github.com/user-attachments/assets/170221bd-629c-4c5b-a4bf-57bada2625e1" />

<sub><em>Navigated to the <code>/var/log</code> directory and verified the current working directory using the <code>pwd</code> command.</em></sub>

---

# Step 2 - View Available Log Files

```bash
ls

ls -lh
```

Displayed the available log files and viewed detailed file information including permissions, ownership, size, and modification dates.

### Screenshot

<img width="843" height="137" alt="image" src="https://github.com/user-attachments/assets/08fa2987-be00-4985-b599-8cee3a5bb26b" />

<sub><em>Listed the available log files using <code>ls</code> and displayed detailed file information with <code>ls -lh</code> to identify logs available for review.</em></sub>

---

# Step 3 - Review the Beginning of the Log

```bash
head keybagd.log.1
```

Displayed the first several entries within the selected log file to observe how events are recorded and organized.

### Screenshot

<img width="851" height="198" alt="image" src="https://github.com/user-attachments/assets/31cabd4a-a981-4a4f-ac23-6d1c4100f554" />


<sub><em>Used the <code>head</code> command to review the beginning of the log file and examine the initial recorded system events.</em></sub>

---

# Step 4 - Review the End of the Log

```bash
tail keybagd.log.2
```

Displayed the most recent log entries to review the latest recorded system activity.

### Screenshot

<img width="857" height="310" alt="image" src="https://github.com/user-attachments/assets/b181986b-133e-42b2-b28c-4d9a957e380b" />


<sub><em>Displayed the most recent log entries using the <code>tail</code> command to review current system activity.</em></sub>

---

# Step 5 - Browse a Log File

```bash
less keybagd.log.3
```

Opened the log file using the `less` command, allowing efficient navigation through a large text file without loading the entire file into memory.

### Screenshot

<img width="859" height="660" alt="image" src="https://github.com/user-attachments/assets/7dd32820-8096-4cad-804d-6e93d2510307" />


<sub><em>Opened the log file using the <code>less</code> command to efficiently browse and review large log files.</em></sub>

---

# Step 6 - Display the First Twenty Log Entries

```bash
cat keybagd.log.3 | head -20
```

Combined the `cat` and `head` commands using a pipe (`|`) to display only the first twenty lines of the selected log file.

### Screenshot

<img width="851" height="198" alt="image" src="https://github.com/user-attachments/assets/8489d244-0d81-44cf-bfe8-33f73ec6e03f" />


<sub><em>Demonstrated command piping by combining <code>cat</code> and <code>head</code> to display the first twenty lines of the selected log file.</em></sub>

---

# Step 7 - Search Log Entries Using `grep`

```bash
grep -i "failed" keybagd.log.3
```

Used the grep command with the -i (case-insensitive) option to search the selected log file for entries containing the keyword "failed."
### Screenshot

<img width="860" height="654" alt="image" src="https://github.com/user-attachments/assets/78f367a6-2620-4ced-a8ea-f738abc226d0" />

<sub><em>Performed a case-insensitive search using <code>grep -i "failed" keybagd.log.3</code> to quickly identify log entries containing the keyword <code>failed</code>. This technique is commonly used during troubleshooting and security investigations to isolate relevant events from large log files.</em></sub>

---

# Skills Learned

Throughout this lab I gained practical experience locating and reviewing Linux system log files using common command-line tools. I learned how to inspect both historical and recent log entries, efficiently navigate large log files, and use command piping to filter output. These foundational log analysis skills are essential for troubleshooting, system administration, and cybersecurity investigations where reviewing logs is often the first step in identifying system events and potential security issues.

---

# Key Takeaways

- Located Linux system log files
- Reviewed log contents using multiple command-line tools
- Navigated large log files efficiently
- Practiced command piping
- Improved Linux command-line proficiency
- Developed foundational log analysis skills used in cybersecurity and system administration
