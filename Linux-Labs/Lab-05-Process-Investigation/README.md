# Lab 05 - Process Investigation

## Objective

Show how to identify, analyze, and investigate running processes on a macOS system using terminal commands. This lab demonstrates how process monitoring helps administrators and security professionals understand system activity, identify unusual behavior, and support incident response investigations.

## Commands Used

- ps
- ps aux
- ps -e
- top
- grep

## Steps Performed

1. Used the `ps` command to display currently running processes associated with the active terminal session.

2. Used the `ps aux` command to display detailed information about all running processes, including the user account associated with each process and resource usage.

3. Used the `ps -e` command to display all currently running processes on the macOS system.

4. Reviewed process information including Process ID (PID), terminal session, CPU time, and command name.

5. Reviewed running processes to identify normal system services and active applications.

6. Used the `top` command to view real-time process activity and monitor system resource usage.

7. Used the `grep` command to filter process output and locate specific processes of interest.

8. Analyzed process information to understand how system activity can be monitored and investigated.

## Results

Successfully identified and reviewed active system processes using macOS terminal commands. Demonstrated the ability to gather process information, analyze running services, and understand how process investigation supports system monitoring and cybersecurity analysis.

## Security Concepts Demonstrated

### Process Enumeration

Identifying running processes provides visibility into system activity and can help detect unauthorized or suspicious applications.

### Incident Response

Process investigation is commonly performed during security investigations to identify potentially malicious activity.

### Threat Detection

Reviewing running processes can help analysts identify abnormal behavior, unknown programs, or unauthorized execution.

## Skills Demonstrated

- macOS/Linux Process Management
- Command-Line Investigation
- System Monitoring
- Process Enumeration
- Security Analysis Fundamentals
- Technical Documentation

## Screenshot

<img width="846" height="276" alt="image" src="https://github.com/user-attachments/assets/d99f14ae-505d-4f2e-b403-77a2e3a56064" />

<img width="842" height="180" alt="image" src="https://github.com/user-attachments/assets/ed261501-2f1f-453d-92a8-a4d1051a8698" />

<sub><em>In the above 2 screenshots I performed process enumeration using the `ps`, `ps aux`, and `ps -e` commands to identify active processes, process ownership, resource usage, and system activity. This information provides visibility into running services and applications, which is a foundational step in system monitoring, threat detection, and incident response investigations.</em></sub>

<img width="849" height="293" alt="image" src="https://github.com/user-attachments/assets/329891d6-51f3-4855-acff-5881b0422e01" />

<sub><em>Used the `top` command to monitor real-time system activity, review running processes, and analyze resource usage including CPU and memory consumption.</em></sub>

<img width="852" height="184" alt="image" src="https://github.com/user-attachments/assets/b87aaa2f-7e10-490e-8726-807f64507d0b" />

<sub><em>Used the `grep` command with process output to filter and identify specific running processes of interest. Commands such as `ps aux | grep Terminal`, `ps aux | grep launchd`, and `ps aux | grep zsh` were used to search for specific processes within system activity data. The command `ps aux | grep "[T]erminal"` was used to locate the Terminal process while preventing the `grep` command itself from appearing in the results.</em></sub>

## Lessons Learned

Understanding running processes is an important part of system administration and cybersecurity. Process investigation provides visibility into system behavior and helps security professionals identify potential threats during monitoring and incident response activities.
