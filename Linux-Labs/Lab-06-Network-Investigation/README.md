# Lab 06 - Network Investigation

## Objective

Learn how to investigate network configuration, active connections, and network activity using macOS terminal commands. This lab demonstrates how network visibility helps administrators and security professionals troubleshoot systems, identify active connections, and support security investigations.

## Commands Used

- ifconfig
- ipconfig getifaddr
- netstat
- ping
- nslookup
- traceroute

## Steps Performed

1. Used the `ifconfig` command to view network interface information and identify available network adapters configured on the system.

2. Reviewed network interface details including assigned IP addresses, interface status, and network configuration information.

3. Used the `ipconfig getifaddr en0` command to retrieve the current IP address assigned to the primary network interface.

4. Used the `netstat -an` command to display active network connections and listening ports on the system.

5. Reviewed active connections to understand how applications communicate across the network.

6. Used the `ping` command to test connectivity between the local machine and a remote host.

7. Used the `nslookup` command to query DNS information and identify how domain names resolve to IP addresses.

8. Used the `traceroute` command to analyze the network path between the local machine and a destination host.

9. Reviewed network information to understand how visibility into connections and traffic can assist with troubleshooting and security investigations.

## Results

Successfully gathered network information, identified active connections, tested connectivity, reviewed DNS resolution, and analyzed network paths using macOS terminal tools. Demonstrated foundational network investigation skills used in system administration and cybersecurity analysis.

## Security Concepts Demonstrated

### Network Visibility

Understanding network configuration and active connections helps identify normal system behavior and potential anomalies.

### Connection Analysis

Reviewing active connections and listening ports can help identify unexpected services or suspicious activity.

### DNS Investigation

DNS analysis helps security professionals understand how systems resolve and communicate with external resources.

### Troubleshooting & Incident Response

Network investigation commands provide valuable information during technical troubleshooting and security investigations.

## Skills Demonstrated

- Network Configuration Analysis
- IP Address Identification
- Network Troubleshooting
- DNS Investigation
- Connection Analysis
- Command-Line Networking Tools
- Security Documentation

## Screenshot

<sub><em>Terminal output showing network investigation commands used to analyze network configuration, active connections, connectivity, DNS resolution, and network paths.</em></sub>

<img width="570" height="457" alt="image" src="https://github.com/user-attachments/assets/d1ad2de4-cd7a-4a37-b1c8-dfbfe7aed728" />

<sub><em>Using the `ifconfig` command to examine the system's network interfaces and review network configuration details, including interface status, IP addressing, and connectivity information. This command provides visibility into how the system is configured to communicate across a network.</em></sub>

<img width="570" height="457" alt="image" src="https://github.com/user-attachments/assets/6d6e0dc0-50bd-4033-b016-3f5ae4c17f73" />

<sub><em>Using the `ipconfig getifaddr en0` command to retrieve the IPv4 address assigned to the system's primary network interface, confirming the device's active network configuration. Followed by the `netstat -an` command to display active network connections and listening ports, providing visibility into current network communication and connection states.</em></sub>

<img width="423" height="111" alt="image" src="https://github.com/user-attachments/assets/b4d4a30a-29ef-4b77-b8b1-aa63d0df8550" />
<img width="469" height="50" alt="image" src="https://github.com/user-attachments/assets/f057f78f-e09f-4bbf-94d3-f70cd5475c3a" />

<sub><em>In the 2 screenshots above I used the `ping google.com` command to test network connectivity between the local system and a remote host by sending ICMP Echo Request packets. The output confirmed successful communication by displaying packet transmission and receipt, response times, packet loss statistics, and round-trip latency measurements (minimum, average, maximum, and standard deviation).</em></sub>

<img width="509" height="399" alt="image" src="https://github.com/user-attachments/assets/b8e9c2e5-dc9b-44fb-8040-de78cc56eb6e" />

<sub><em>Using the `nslookup google.com` command to query the Domain Name System (DNS) and resolve the domain name to its corresponding IP address. Followed by the `traceroute google.com` command to trace the network path between the local system and a remote host by identifying each intermediate router (hop) along the route. The output displays the sequence of network hops and their response times, providing insight into packet routing, network latency, and potential points of delay.</em></sub>


## Lessons Learned

Network visibility is a critical component of cybersecurity. Understanding how systems communicate and how to investigate network activity provides a foundation for detecting abnormal behavior and investigating potential security incidents.

## NOTE:

Certain network identifiers (IP addresses, IPv6 addresses, subnet information, and MAC addresses) have been redacted from screenshots to protect personal network information while preserving the educational value of the lab.
