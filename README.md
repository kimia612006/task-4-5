 Task 4 - Firewall Configuration and Testing

Objective
To configure Windows Firewall to block and allow specific traffic, test the rules, and understand how firewalls filter network traffic.
 Tools Used
- Windows Defender Firewall with Advanced Security
- Command Prompt / PowerShell
- Telnet Client (for testing)
- Test-NetConnection (PowerShell command)

---

 Steps Performed
Checked existing rules** in Windows Firewall and took a screenshot.
2. Enabled Telnet Client  on Windows:
cmd
dism /online /Enable-Feature /FeatureName:TelnetClient
Created a new inbound rule in Windows Firewall to block TCP port 23 (Telnet).

Tested the rule:

Using telnet localhost 23



Removed the test rule to restore firewall to original state.

What I Learned
The difference between inbound and outbound rules

How to block insecure services like Telnet

How to test firewall rules from both Windows and WSL

How Windows Firewall filters traffic at the port level

 Files in This Repo
README.md — Documentation of the task

