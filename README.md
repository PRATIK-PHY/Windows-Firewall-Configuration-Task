Windows Firewall Configuration Task

🛡️ Objective
The objective of this task is to configure and test basic firewall rules on a Windows machine to understand how to allow or block network traffic.

🛠️ Tools Used
Windows Defender Firewall with Advanced Security: The built-in firewall management tool in Windows.

PuTTY (or similar tool): Used to test network connections.


⚙️ Steps for Configuration and Testing
The following steps were performed to complete the task:

Open Windows Firewall: Accessed Windows Defender Firewall with Advanced Security via the Start Menu.

View Current Rules: Navigated to the Inbound Rules and Outbound Rules sections to review the existing configurations.

Add a Rule to Block Inbound Traffic:

Opened the New Inbound Rule Wizard.

Selected Port as the rule type.

Configured the rule to block TCP connections on Port 23 (Telnet).

Set the action to Block the connection.

Applied the rule to all profiles (Domain, Private, Public).

Named the rule "Block Telnet Port 23".

Test the Rule:

Used a Telnet client (like PuTTY) to attempt a connection to localhost on port 23.

The connection was immediately blocked, confirming the rule was working as intended.

Remove the Test Rule:

Returned to the Inbound Rules list.

Right-clicked on the "Block Telnet Port 23" rule and selected Delete to restore the original state.

📝 Summary: How Firewalls Filter Traffic
A firewall acts as a digital security guard for a computer, controlling network traffic based on a set of pre-defined rules. It inspects data packets (both incoming and outgoing) and decides whether to allow them through or block them. This filtering is typically based on:

IP Address: The source and destination of the traffic.

Port Number: The specific service or application the traffic is for (e.g., port 80 for web pages, port 443 for secure web pages).

Protocol: The type of communication being used (e.g., TCP or UDP).

By filtering traffic, a firewall protects a system from unauthorized access and potential threats, ensuring that only intended and secure connections are established.
