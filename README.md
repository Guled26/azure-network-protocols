<p align="center">
<img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>Network Security Groups (NSGs) and Inspecting Traffic Between Azure Virtual Machines</h1>
In this tutorial, we observe various network traffic to and from Azure Virtual Machines with Wireshark as well as experiment with Network Security Groups. <br />


<h2>Video Demonstration</h2>

- ### [YouTube: Azure Virtual Machines, Wireshark, and Network Security Groups](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Various Command-Line Tools
- Various Network Protocols (SSH, RDH, DNS, HTTP/S, ICMP)
- Wireshark (Protocol Analyzer)

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)
- Ubuntu Server 20.04

<h2>High-Level Steps</h2>

Step 1: Create Network Security Groups (NSGs)

In the Azure portal, navigate to "Networking" and create a new NSG for your VMs.
Define inbound and outbound security rules to control traffic.

Step 2: Define Security Rules

In the NSG settings, create inbound rules specifying allowed traffic sources, destination ports, and protocols (e.g., TCP, UDP).
Define outbound rules to manage traffic leaving the VMs.

<h2>Actions and Observations</h2>

<p>
<img src="https://learn.microsoft.com/en-us/azure/bastion/media/bastion-nsg/figure-1.png"/>
</p>
<p>
Step 3: Associate NSGs with VMs

Attach the NSG to the network interface (NIC) or subnet associated with each VM.
This enforces the defined security rules for those VMs.

Step 4: Default Rules

By default, NSGs deny all inbound and outbound traffic.
Create rules that explicitly allow necessary traffic, such as HTTP (port 80) or SSH (port 22).

Step 5: Inspect Traffic

Monitor traffic flows through NSGs using Azure Monitor or Network Watcher.
Use Azure Security Center for threat detection and monitoring.
</p>
<br />

<p>
<img src="https://1138blog.files.wordpress.com/2021/08/image.png?w=1024"/>
</p>
<p>
Step 6: Test Connectivity

Validate that your NSG rules allow the desired traffic between VMs and external sources.
Use tools like telnet or ping for testing.

Step 7: Logging and Alerts

Enable logging for NSG rules to capture traffic data.
Set up alerts for suspicious or unauthorized traffic patterns.
</p>
<br />

<p>
<img src="https://learn.microsoft.com/en-us/azure/iot-central/core/media/howto-configure-rules/conditions.png"/>
</p>
<p>
Step 8: Review and Refine Rules

Periodically review NSG rules and refine them based on changing network requirements and security needs.

Step 9: Documentation

Maintain documentation of NSG configurations, rules, and any changes made.
Ensure the documentation is accessible to relevant team members.

Step 10: Compliance and Auditing

Regularly audit NSG configurations to ensure compliance with security policies and regulations.
Make adjustments as needed to address security vulnerabilities.
</p>
<br />
