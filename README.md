# 30 Days SOC Automation Challenge
 ELK Stack SOC automation using Fleet and OS Ticketing Server

## Day 1: Logical Diagram

🚀 Embarking on MYDFIR 30-Days SOC Challenge! by my mentor Steven ([link](https://lnkd.in/dRGfScbr)) 🚀  
I'm thrilled to announce that I'll be diving into an intensive Security Operations Center (SOC) simulation, where I'll be provisioning and managing a complex environment on VULTR Cloud. This project is designed to enhance my skills as a SOC Analyst by replicating real-world scenarios and challenges.

### Key Components of the Environment:
- 🖥️ **Windows Server with RDP enabled**: A critical asset in many infrastructures, ripe for security monitoring and attack vector simulation.
- 🎛️ **Fleet Server**: Centralizing management and monitoring of the environment, a key part of maintaining security posture.
- 🐧 **Ubuntu Server with SSH enabled**: Providing a platform to simulate and detect unauthorized access attempts.
- 📊 **ELK Stack Server**: A powerful tool for log aggregation, analysis, and visualization—essential for incident detection and response.
- 📋 **OS Ticketing Server**: Integrating with incident response processes to track and manage security incidents efficiently.
- 🎯 **Command and Control Server with Kali Linux**: The heart of the simulated attack, representing a persistent threat actor within the network.

What to Expect:  
Over the next 30 days, I’ll be sharing insights, challenges, and key learnings as I simulate attacks and respond to incidents in this environment. This journey promises to be both rigorous and rewarding, offering valuable lessons that I look forward to applying in real-world SOC operations.

Feel free to engage with your thoughts and questions along the way!

FREE $300 Cloud Credit (Vultr): [link](https://lnkd.in/drVeaA5s) - Only applies to new accounts.

---
![SOC LAB Image](https://github.com/Virus192/elk-soc-automation/blob/main/images/SOC%20LAB.jpg)



## [Day 2: ELK Stack Deep Dive](https://github.com/Virus192/Day-2-ELK-Stack-Deep-Dive)

🚀 **Day 2 of MYDFIR 30 Days SOC Challenge: We took a Deep Dive into the ELK Stack** 🚀  
Today we focus on the ELK Stack—a cornerstone technology in Security Operations Centers (SOC) for effective log management and threat analysis. 

### Technical Overview of the ELK Stack:
1. **Elasticsearch** 🗄️  
   **Function**: A highly scalable search and analytics engine.  
   **Role in SOC**: Stores and indexes vast amounts of log data, enabling quick search and real-time analysis of security events.

2. **Logstash** 🛠️  
   **Function**: A server-side data processing pipeline.  
   **Role in SOC**: Ingests data from various sources, transforms it, and sends it to Elasticsearch for indexing.

3. **Kibana** 📊  
   **Function**: A visualization and exploration tool.  
   **Role in SOC**: Provides interactive dashboards and visualizations of the data stored in Elasticsearch.

4. **Beats** 🐝  
   **Function**: Lightweight data shippers.  
   **Role in SOC**: Collects data from various sources and forwards it to Logstash or Elasticsearch for processing.

### Significance of ELK Stack in the SOC Project:
- **Centralized Log Management**: Aggregates logs from diverse sources into a single repository.
- **Real-Time Threat Detection**: Facilitates the swift identification of suspicious activities through real-time processing.
- **Scalability and Flexibility**: Handles large volumes of data, allowing the SOC to grow.
- **Customizable Dashboards**: Empowers SOC analysts to create tailored dashboards for critical security metrics.

---
![SOC LAB Image](https://raw.githubusercontent.com/Virus192/Day-2-ELK-Stack-Deep-Dive/main/images/1_EElZCCfA9S0kgABEDi5sOw.png)


## [Day 3: Building a Secure Elasticsearch Deployment](https://github.com/Virus192/Day-3-Building-a-Secure-Elasticsearch-Deployment)

🌟 **Day Three of #MYDFIRSOCChallenge: Building a Secure Elasticsearch Deployment** 🌟  
Special Thanks to MYDFIR for this exciting challenge!

Today was all about diving deep into the world of Elasticsearch Consulting! 🎯 As part of the #30DaysSOCChallenge, I had the opportunity to set up and secure an Elasticsearch instance, and it was an exciting ride. 🚀

### What's on the Plate?
- **Installed Elasticsearch on a robust Ubuntu 22.04 LTS environment**. 🐧
- **Ensured a secure deployment by implementing a well-configured firewall**. 🔒
- **Deployed within a VPC 2.0 on Vultr for enhanced network security**. 🌐

### Why Does This Matter?
Elasticsearch is a powerful tool in the SOC toolkit, enabling efficient search, analysis, and visualization of log data. However, ensuring its secure deployment is crucial to avoid becoming a target of the very threats we seek to defend against.

### Key Takeaways:
- **Ubuntu 22.04 LTS provides a stable and secure foundation for hosting Elasticsearch, minimizing vulnerabilities from the OS level.**
- **A secured firewall setup is non-negotiable—it keeps unwanted visitors at bay, protecting our data and services.**
- **Leveraging VPC 2.0 in Vultr adds an extra layer of network segmentation and security, isolating our deployment from potential threats.**

As I progress through this challenge, I'm constantly reminded of the importance of robust security practices in every layer of deployment. Looking forward to seeing how this setup will empower our security operations moving forward! 💪

FREE $300 Cloud Credit (Vultr): [Link](https://lnkd.in/drVeaA5s) - Only applies to new accounts.

![Elasticsearch Setup](https://raw.githubusercontent.com/Virus192/elk-soc-automation/main/images/photo_5960977688871158764_w.jpg)

## [Day 4: Elasticsearch Security Configuration](https://github.com/Virus192/Day-4-Elasticsearch-Security-Configuration)

---------------------------

### 🌟 It's Day 4 of the MYDFIR 30-Day SOC Automation Challenge.
 Here is our Task for today: Kibana Installation & Configuration 🌟
 Today's journey was all about setting up and configuring Kibana to visualize and analyze our Elasticsearch data. Here's how it all went down:

The generated password for the elastic built-in superuser is: `OK6A_2wP9DZql=hYsc1M`

If this node should join an existing cluster, you can reconfigure this with:
`/usr/share/elasticsearch/bin/elasticsearch-reconfigure-node --enrollment-token <token-here>`
after creating an enrollment token on your existing cluster.

You can complete the following actions at any time:

- Reset the password of the elastic built-in superuser with:
  `/usr/share/elasticsearch/bin/elasticsearch-reset-password -u elastic`.

- Generate an enrollment token for Kibana instances with:
  `/usr/share/elasticsearch/bin/elasticsearch-create-enrollment-token -s kibana`.

- Generate an enrollment token for Elasticsearch nodes with:
  `/usr/share/elasticsearch/bin/elasticsearch-create-enrollment-token -s node`.

### NOT starting on installation, please execute the following statements to configure Elasticsearch service to start automatically using systemd
```bash
sudo systemctl daemon-reload
sudo systemctl enable elasticsearch.service
```
![SOC](https://raw.githubusercontent.com/Virus192/elk-soc-automation/main/images/photo_5965442483469009319_w.jpg)

## [Day 5: Deploying a Windows Server on Vultr Cloud](https://github.com/Virus192/Day-5-Deploying-a-Windows-Server-on-Vultr-Cloud)

🌟 **Day 5 of MYDFIR 30 Days SOC Challenge: Deploying a Windows Server on Vultr Cloud** 🌟

Today, I deployed a Windows Server on Vultr Cloud, moving it out of VPC 2.0 for public accessibility.

## Quick Steps

1. **Login to Vultr Cloud** and click on the **Deploy +** button.
2. **Choose Server Type:** Cloud Compute — Shared CPU.
3. **Select Plan:** 55GB SSD, 1 vCPU, 2GB memory.
4. **Deploy:** Click **Deploy Now** and wait 5-7 minutes.
5. **Access:** Use the provided credentials to log in.

Deploying a Windows Server on Vultr Cloud is a simple process, ideal for making your server publicly accessible while keeping costs low.


![Windows Server Deployment](https://raw.githubusercontent.com/Virus192/elk-soc-automation/main/images/1_VCKRGZAd1IWFjfHcdCKCDg.png)

## [Day 6: Introduction to Fleet Server and Elastic Agent](https://github.com/Virus192/Day-6-Introduction-to-Fleet-Server-and-Elastic-Agent)

 🌟 **Day 6 of MYDFIR 30 Days SOC Challenge: Exploring Fleet Server and Elastic Agent** 🌟

Today’s focus is on mastering the centralized management of Elastic Agents using Fleet Server, an essential tool for large-scale environments.

Imagine deploying Elastic Agents on 100 Windows machines to monitor PowerShell logs, only to realize they’re not forwarding logs to your Elasticsearch instance. What would you do? Instead of manually reconfiguring each endpoint, you could use Fleet Server to handle everything centrally.

## Key Components

### Elastic Agent

- A unified tool for monitoring logs, metrics, and other data types, with policies you can update remotely.
- Two modes of installation:
  - **Fleet Managed Mode:** Centralized management
  - **Standalone:** Manual setup

### Fleet Server

- The backbone of centralized agent management, allowing you to:
  - Deploy policies
  - Add integrations
  - Update agents across all endpoints with ease

## Why Use Fleet Server?

- **Centralized Management:** Control agent policies and integrations from one dashboard.
- **Seamless Updates:** Easily push updates to all agents at once, saving hours of manual work.
- **Simplified Unenrollment:** Unenroll agents with just a few clicks, eliminating the need to touch every machine.

Leveraging Fleet Server simplifies your SOC operations, ensuring efficient data collection and security monitoring across your environment.

![insert image here](https://raw.githubusercontent.com/Virus192/SOC-AUTOMATION-ELK-STACK/refs/heads/main/images/a.png)


## [Day 7: Setting Up Elastic Fleet Server and Enrolling Windows Server](https://github.com/Virus192/Day-7-Setting-Up-Elastic-Fleet-Server-and-Enrolling-Windows-Server)

🌟 **Day 7 of MYDFIR 30 Days SOC Challenge: Setting Up Elastic Fleet Server and Enrolling a Windows Server Using Elastic Agent** 🌟

Today's challenge dives into centralizing the management and monitoring of multiple servers using Elastic Fleet and Elastic Agent. We set up a Fleet Server on Vultr, installed an Elastic Agent on a Windows Server, and enrolled it into our fleet for seamless monitoring.

## Steps to Achieve This:

### 1. Create Fleet Server on Vultr

- Deployed a Fleet Server using Ubuntu 22.04 LTS on Vultr.
- Selected **Optimized Cloud Compute** for enhanced performance and security.

### 2. Configure Fleet in Elastic

- Accessed Elastic's GUI, navigated to the **Fleet Management** tab, and added a new Fleet Server.
- Generated the **Fleet Service Policy** and **Service Token** required for connecting the Elastic Agent.

### 3. Install Elastic Agent on Fleet Server

- SSH'd into the Fleet Server, updated the system, and installed the Elastic Agent using the Elastic GUI-generated command.
- Configured firewall rules to allow necessary traffic on ports 9200 and 8200.

### 4. Enroll Windows Server

- Installed the Elastic Agent on a Windows Server via PowerShell.
- The Windows Server was successfully enrolled and connected to the Fleet for centralized monitoring.

## Outcome

Successfully deployed a Fleet Server and enrolled a Windows Server, enabling real-time monitoring of logs and metrics through the Elastic Stack. This setup enhances our SOC’s ability to maintain operational visibility and detect potential threats.

![insert image here](image.jpg)


## [Day 8: Installing Sysmon on a Windows Server](https://github.com/Virus192/Day-8-Installing-Sysmon-on-a-Windows-Server)


**Day 8 of MYDFIR 30 Days SOC Challenge: Installing Sysmon for Advanced Telemetry** 🚀

Today’s focus was on enhancing our visibility into system activity by installing Sysmon (System Monitor) on a Windows Server. Sysmon is a critical tool for SOC environments, providing detailed telemetry that aids in detecting suspicious activities and bolstering security.

## Step-by-Step Highlights

1. **Download Sysmon and Configuration File**
   - Downloaded Sysmon and the popular Sysmon Olaf Configuration file from GitHub, which guides what system events to log.

2. **Install Sysmon**
   - Installed Sysmon using PowerShell and configured it with the downloaded configuration file.

3. **Verify Telemetry**
   - Verified telemetry by checking the Sysmon logs in the Event Viewer, ensuring it captures key activities such as process creation and network connections.

Sysmon is now actively monitoring the Windows Server, providing valuable insights into system events. Another day, another tool deployed in our SOC environment—helping us stay one step ahead of potential threats. 💻🔒

Stay tuned for more security setups!

![insert image here](image.jpg)

## [Day 9: Introduction to Sysmon](https://github.com/Virus192/Day-9-Introduction-to-Sysmon)

 🌟 **Day 9 of MYDFIR 30 Days SOC Challenge: Introduction to Sysmon** 🌟

Today's focus was all about enhancing endpoint visibility with Sysmon—a crucial tool for security analysts in detecting and responding to advanced threats. In the world of cybersecurity, having detailed logs of system activities is essential, and Sysmon steps in to provide that extra layer of monitoring.

## 🔍 What is Sysmon?

Sysmon, part of Microsoft's Sysinternals Suite, is a tool that logs critical system events like process creation, network connections, and file modifications. It goes beyond default Windows logging by offering highly detailed telemetry that allows SOC analysts to track malicious activity in real time. Using a customizable configuration file, Sysmon can fine-tune the events you want to monitor, making it an invaluable asset during investigations.

## 💡 Key Capabilities

- **Process Creation Logging**: Tracks newly created processes with detailed command-line information.
- **File Hashing**: Logs file hashes (SHA1, MD5, etc.) to aid in threat intelligence and OSINT.
- **Network Connection Monitoring**: Records inbound/outbound connections, crucial for detecting C2 activities.
- **Dynamic Rule Filtering**: Focus on the most relevant events by customizing rule-based filters.

Sysmon empowers SOC teams to gain deeper insights into endpoint activities, offering the ability to detect attacks early and correlate events across different logs using unique Process GUIDs.

Stay tuned for more insights tomorrow as we dive deeper into endpoint monitoring with Sysmon! 💪

![insert image here](image.jpg)

## [Day 10: Ingesting Sysmon and Windows Defender Logs into Elasticsearch](https://github.com/Virus192/Day-10-Ingesting-Sysmon-and-Windows-Defender-Logs-into-Elasticsearch)


🚀 **Day 10 of MYDFIR 30 Days SOC Challenge: Ingesting Sysmon and Windows Defender Logs into Elasticsearch** 🚀

Today’s focus was on enhancing visibility into our Windows environment by setting up log ingestion for Sysmon and Windows Defender into Elasticsearch. This process allows for powerful log analysis and real-time threat detection within the SOC.

#### Key Steps:

🛠️ **Elastic Integrations**: Configured Sysmon and Windows Defender logs using Elastic’s GUI. For each integration:
- Named and described the log sources, using Event Viewer to locate the correct channels.
- Specified event IDs for Windows Defender to capture critical security actions, such as detecting malware and real-time protection status.

🔒 **Firewall Configuration**: Ensured logs could be transmitted to Elasticsearch by setting up firewall rules to allow TCP traffic on port 9200.

🔍 **Log Verification**: Used Elastic’s Discover feature to verify that the logs were being ingested properly, focusing on key event IDs (like `winlog.event_id: 5001` for Windows Defender).

With Sysmon and Windows Defender logs now integrated, we’ve built a solid foundation for monitoring and responding to security events within our Windows infrastructure.

![insert image here](https://raw.githubusercontent.com/Virus192/SOC-AUTOMATION-ELK-STACK/refs/heads/main/images/photo_5981008608885852041_w.jpg)

## [Day 11: Fortify Your Digital Walls with Brute Force Attack Prevention](https://github.com/Virus192/Day-11-Fortify-Your-Digital-Walls-with-Brute-Force-Attack-Prevention)

🔐 **Day 11 of MYDFIR 30 Days SOC Challenge: Fortify Your Digital Walls with Brute Force Attack Prevention** 🔐

Today’s insight centers around **Brute Force Attacks** — the digital equivalent of trying every key in the world to unlock your door. Hackers use this method to guess passwords and gain unauthorized access to accounts and systems.

### Types of Brute Force Attacks 🔍
1. **Simple Brute Force**: Trying all possible character combinations.
2. **Dictionary Attack**: Using a list of common words or passwords.
3. **Credential Stuffing**: Reusing passwords leaked from data breaches.

### How to Defend Yourself ⚔️
1. **Strong, Unique Passwords**: Use long, complex passwords or passphrases.
2. **Multi-Factor Authentication (MFA)**: Add a second layer of security.
3. **Password Manager**: Safely store and manage unique passwords.
4. **Stay Vigilant**: Watch out for phishing attempts.
5. **Regular Updates**: Change passwords regularly, especially after breaches.

### Common Brute Force Tools 💻
While tools like **Hydra**, **Hashcat**, and **John the Ripper** exist, they should only be used ethically, with permission, for security testing.

Brute force attacks are persistent but preventable. Stay informed, protect your data, and keep the hackers out! 🌐✨

## [Day 12: Setting Up an SSH Server and Analyzing Authentication Logs](https://github.com/Virus192/Day-12-Setting-Up-an-SSH-Server-and-Analyzing-Authentication-Logs)

🔒 **Day 12 of MYDFIR 30 Days SOC Challenge: Setting Up an SSH Server and Analyzing Authentication Logs** 🔒

Today, we focused on setting up an SSH server on Vultr and analyzing its authentication logs for better security monitoring.

### Deploying Your SSH Server 🌐
1. **Log In** to your Vultr account and click “Deploy.”
2. **Select Specifications**:
   - **Type**: Cloud Compute — Shared CPU
   - **Location**: Choose your preferred region
   - **Image**: Ubuntu 24.04 LTS x64
   - **Plan**: Regular Cloud Compute (25GB SSD, 1 vCPU, 1GB Memory)
3. **Name and Deploy** your server.

### Accessing Your Server 💻
- **SSH Access**: Use PowerShell with the provided credentials.
- **Update System**:
   ```bash
   apt-get update && apt-get upgrade
   
![insert image here](https://raw.githubusercontent.com/Virus192/SOC-AUTOMATION-ELK-STACK/refs/heads/main/images/photo_5987967405093143047_w.jpg)

## [Day 13: Elastic Agent Installation on Ubuntu for Server Monitoring](https://github.com/Virus192/Day-13-Elastic-Agent-Installation-on-Ubuntu-for-Server-Monitoring)

🚀**Day 13 of MYDFIR 30 Days SOC Challenge:: Elastic Agent Installation on Ubuntu for Server Monitoring** 🚀

Today, we're diving into setting up an **Elastic Agent** on your Ubuntu server to help monitor performance and security. 🌐 This powerful tool allows you to centralize logs, monitor in real-time, gain security insights, and scale easily as your infrastructure grows. 💡

## Steps

1. **Elastic Environment Setup**:
   - Log into your Elastic GUI
   - Navigate to "Fleet" under "Management"

2. **Create Agent Policy**:
   - Build a custom policy for your server (e.g., `Ubuntu-Server-Policy`)

3. **Generate Installation Command**:
   - Use the command generated in "Fleet" for your Linux server

4. **Install Agent on Ubuntu**:
   - SSH into your server
   - Execute the installation command

5. **Verify the Installation**:
   - Check for incoming logs in the "Discover" tab of Elastic

🎉 **Congrats**! You now have a robust monitoring solution for your server. 

Stay tuned for tomorrow's guide, where we'll dive into creating **brute force alerts** and a **dashboard** for attack visualization. 👀

**Almost there—keep pushing!** 🔥

![Alt text](https://raw.githubusercontent.com/Virus192/SOC-AUTOMATION-ELK-STACK/refs/heads/main/images/photo_5989808863731369922_w.jpg)

## [Day 14: SSH Brute Force Alerts with Elastic](https://github.com/Virus192/Day-14-SSH-Brute-Force-Alerts-with-Elastic)

🚨🔐**Day 14 of MYDFIR 30 Days SOC Challenge:: SSH Brute Force Alerts with Elastic** 🚨🔐


Today’s mission: setting up **SSH brute force attack** alerts in Elastic to safeguard your servers. These attacks involve hackers guessing passwords to gain access. Let’s get proactive with alerts and visual dashboards!

**Why Monitor SSH Attacks?**
- **Early Detection**: Spot attacks quickly for fast action.
- **Pattern Insights**: Learn from repeated attacks.
- **System Protection**: Prevent overload from constant login attempts.

**Setting Up Alerts ⚠️**
- Track failed login attempts, target accounts, and IPs.
- Use Elastic to create an alert based on these conditions.
- Customize thresholds for precision.

**Visual Dashboard** 🌍
Create a map in Elastic to track where the attacks come from globally.

**Wrap-Up 🛡️**
With alerts and dashboards in place, you can detect and visualize attacks, keeping your systems safe. Stay secure! 💪🔒

![Alt text](https://raw.githubusercontent.com/Virus192/SOC-AUTOMATION-ELK-STACK/refs/heads/main/images/photo_5994510577315202212_w.jpg)

## [Day 15: Protecting Your Network from RDP Abuse](https://github.com/Virus192/Day-15-Protecting-Your-Network-from-RDP-Abuse)

🖥️**Day 15 of MYDFIR 30 Days SOC Challenge:: Protecting Your Network from RDP Abuse** 🔒

On our journey through cybersecurity, today we're diving into one of the most abused tools in the cyber world: **Remote Desktop Protocol (RDP)**. RDP allows users to remotely access computers, making IT troubleshooting a breeze. However, when exposed, it can become a hacker’s doorway.

Attackers often use methods like **brute force attacks** or **credential theft** to break in through RDP, allowing them to move across networks, steal data, or deploy ransomware. 😨

## 🔍 Finding Exposed RDP Endpoints:
Using tools like **Shodan** or **Censys**, you can scan for open RDP services on port 3389. These tools help you spot any endpoints that may be vulnerable and take action to secure them.

## 🛡️ Protecting Yourself from RDP Abuse:
- **Turn off RDP** when not needed.
- Use **Multi-Factor Authentication (MFA)** to add an extra layer of security.
- **Restrict access** using firewalls or VPNs.
- **Enforce strong passwords** and disable default admin accounts.

Remember, a layered defense approach is essential to keeping your systems safe. Secure your RDP access today, and stay vigilant!

![Alt text](https://raw.githubusercontent.com/Virus192/SOC-AUTOMATION-ELK-STACK/refs/heads/main/images/photo_5999014176942572320_w.jpg)

## [Day 16: Setting Up Alerts for RDP and SSH Brute Force Attacks on Windows Server ](https://github.com/Virus192/Day-16-Setting-Up-Alerts-for-RDP-and-SSH-Brute-Force-Attacks-on-Windows-Server)

🚨 **Day 16 of MYDFIR 30 Days SOC Challenge: Setting Up Alerts for RDP and SSH Brute Force Attacks on Windows Server** 🚨

Today's focus was on enhancing our Windows Server security by configuring alerts for RDP and SSH brute force attacks using Elastic. Here's a quick rundown of what we accomplished:

**RDP Brute Force Monitoring** 🖥️

- Set up log monitoring in Elastic Discover
- Filtered for Event ID 4625 (failed login attempts)
- Created a search threshold rule for RDP brute force detection

**SSH Brute Force Detection** 🔐

- Crafted a custom detection rule for SSH attempts
- Focused on failed root user login attempts
- Set threshold to 5 failed attempts within a specified timeframe

**Alert Configuration** ⚠️

- Customized rule settings for both RDP and SSH
- Set up alerts to run every 5 minutes with a 5-minute look-back period

**Monitoring Setup** 👀

- Configured the Alerts section for easy viewing of suspicious activities

By implementing these measures, we've significantly boosted our ability to detect and respond to potential brute force attacks on our Windows Server. Remember, staying vigilant and proactive is key to maintaining a robust security posture! 💪🛡️

![Example Image](example.png)

## [Day 17: Building a Comprehensive Dashboard for RDP & SSH Authentication Monitoring ](https://github.com/Virus192/Day-17-Building-a-Comprehensive-Dashboard-for-RDP-SSH-Authentication-Monitoring)

 📊 **Day 17 of MYDFIR 30 Days SOC Challenge: Building a Comprehensive Dashboard for RDP & SSH Authentication Monitoring** 📊

Today, we focused on creating a robust dashboard in Elastic to monitor both RDP and SSH authentication attempts. This visualization tool will help us quickly identify potential security threats and unauthorized access attempts. Here's what we accomplished:

**RDP Failed Authentication Monitoring** 🖥️

- Created a map layer using **Choropleth** to visualize failed RDP attempts by country.
- Used event code **4625** to track failed Windows authentication attempts.

**Successful RDP Login Tracking** ✅

- Set up monitoring for successful RDP logins using event code **4624**.
- Tracked both **Remote Interactive (Type 10)** and **Unlock (Type 7)** events.

**Enhanced Dashboard with Detailed Tables** 📋

- Added tables to display usernames, source IPs, and countries for both failed and successful attempts.
- Created separate tables for SSH and RDP activities.

**Comprehensive View** 🔍

- Combined RDP and SSH monitoring into a single dashboard.
- Provided visual maps and detailed tables for both protocols.

**Insights at a Glance** 💡

- Enabled quick identification of usernames, source IPs, and countries involved in authentication attempts.
- Facilitated easy tracking of total attempts and their outcomes.

By implementing this dashboard, we've significantly improved our ability to monitor, investigate, and respond to suspicious authentication activities across our network. Stay vigilant and keep refining your security measures! 🛡️🔐

![Example Image](https://raw.githubusercontent.com/Virus192/SOC-AUTOMATION-ELK-STACK/refs/heads/main/images/photo_6003690240981714182_w.jpg)

## [Day 18: Understanding Command & Control (C2) in Cyber Attacks ](https://github.com/Virus192/Day-18-Understanding-Command-Control-C2-in-Cyber-Attacks)

🕵️**Day 18 of MYDFIR 30 Days SOC Challenge: Understanding Command & Control (C2) in Cyber Attacks**🕵️

Today, we delved into the world of Command & Control (C2), a crucial component in cyber attacks. Here's what we learned:

**C2 Basics** 📡

- **Definition**: Techniques used by attackers to communicate with compromised systems
- **Purpose**: Allows remote control of victim machines for various malicious activities

**Importance of C2** 🎯

- Maintains access to compromised systems
- Enables execution of commands for further exploitation
- Facilitates data exfiltration and malware deployment

**Popular C2 Tools** 🛠️

- **Metasploit**: Versatile framework for penetration testing
- **Cobalt Strike**: Commercial tool often misused by attackers
- **Sliver**: Open-source framework with multiple communication channels
- **Mythic**: Modern C2 platform with web-based UI and Docker integration

**Spotlight on Mythic** 🔍

- Features web-based interface for easy management
- Uses Docker and Go for efficient deployment
- Supports multiple C2 profiles and communication channels
- Offers payload tracking for precise operations

**Future Plans** 🚀

- Upcoming hands-on setup of a Mythic C2 server
- Practical demonstration of deploying an agent on a Windows server

Understanding C2 is crucial for both attackers and defenders in the cybersecurity landscape. Stay tuned as we prepare to dive deeper into practical C2 operations in our upcoming sessions! 💪🛡️

![Example Image](example.png)

## [Day 19: Mapping a Simulated Attack Path](https://github.com/Virus192/Day-19-Mapping-a-Simulated-Attack-Path)

🗺️**Day 19 of MYDFIR 30 Days SOC Challenge: Mapping a Simulated Attack Path**🗺️

Today, we focused on creating a comprehensive attack diagram to simulate a cyber attack on a Windows Server. This exercise helps us understand the attacker's perspective and strengthens our defense strategies. Here's what we covered:

**Initial Access**🚪
- Simulated RDP brute-force attack using Kali Linux.

**Discovery** 🔍
- Explored basic system reconnaissance commands:
  - `whoami`
  - `ipconfig`
  - `net user`
  - `net group`

**Defense Evasion** 🛡️
- Simulated disabling of Windows Defender.

**Execution** 🚀
- Used PowerShell to download and execute the Mythic Agent.

**Command and Control (C2)** 🕹️
- Established a simulated C2 session using the Mythic Agent.

**Exfiltration** 📤
- Demonstrated data theft by extracting a fake `password.txt` file.

This attack path simulation provides invaluable insights into how attackers operate, helping us build more robust defenses. By understanding each phase, from initial access to data exfiltration, we can better protect our systems and respond effectively to real-world threats.

Stay tuned for our next session, where we'll begin setting up the infrastructure for this simulated attack! 💪🔒

![Example Image](https://raw.githubusercontent.com/Virus192/SOC-AUTOMATION-ELK-STACK/refs/heads/main/images/Copy%20of%20Copy%20of%20MYDFIR-C%26C.drawio.png)

## [Day 20: Setting Up Your Own Mythic C2 Instance](https://github.com/Virus192/Day-20-Setting-Up-Your-Own-Mythic-C2-Instance)

🕵️‍♂️**Day 20 of MYDFIR 30 Days SOC Challenge: Setting Up Your Own Mythic C2 Instance**🕵️‍♂️

Today, we delved into the world of Command and Control (C2) by setting up our own Mythic C2 instance. Here's what we accomplished:

### Cloud Server Setup ☁️
- Deployed an **Ubuntu 22.04 LTS** server on **Vultr**
- Configured with **2 vCPUs, 4GB RAM, and 80GB SSD**

### Server Preparation 🛠️
- Updated and upgraded the system
- Installed **Docker Compose** and **Make**

### Mythic Installation 🚀
- Cloned the Mythic repository from **GitHub**
- Ran the installation script and started Docker

### Firewall Configuration 🔒
- Set up a firewall group in Vultr to control access

### Mythic Web GUI Access 🖥️
- Accessed the Mythic interface via **HTTPS**
- Retrieved login credentials from the server

This hands-on experience with Mythic C2 provides valuable insights into how attackers might establish and maintain control over compromised systems. Remember, always practice in controlled environments and use these tools responsibly!

Stay tuned for our next session, where we'll dive deeper into Kali Linux and create our first Mythic agent! 💪🛡️

![Example Image](https://raw.githubusercontent.com/Virus192/SOC-AUTOMATION-ELK-STACK/refs/heads/main/images/photo_6012391733054260189_w.jpg)

## [Day 21: Simulating a Brute Force Attack with Mythic C2](https://github.com/Virus192/Day-21-Simulating-a-Brute-Force-Attack-with-Mythic-C2)

🕵️‍♂️**Day 21 of MYDFIR 30 Days SOC Challenge: Simulating a Full Attack Chain with Mythic C2**🕵️‍♂️

Today, we conducted a comprehensive simulation of a Brute Force Attack chain using Kali Linux, Mythic C2, and a Windows Server. Here's what we accomplished:

### Attack Phases 🎭
- **Initial Access:** Performed RDP brute-force attack using Crowbar
- **Discovery:** Executed basic reconnaissance commands
- **Defense Evasion:** Disabled Windows Defender
- **Execution:** Deployed Mythic C2 agent on target
- **Command & Control:** Established C2 session
- **Exfiltration:** Retrieved a fake passwords file

### Key Steps 🔑
- Set up a Windows Server with a dummy file
- Created a custom wordlist for brute-forcing
- Generated and deployed a Mythic C2 payload
- Used PowerShell to download and execute the payload
- Interacted with the compromised system via Mythic GUI

### Tools Used 🛠️
- Kali Linux
- Crowbar for RDP brute-forcing
- Mythic C2 framework
- PowerShell for payload execution

This hands-on exercise provided valuable insights into the attacker's perspective, enhancing our understanding of complex attack chains. Remember, always practice ethical hacking and obtain proper authorization before testing any systems!

Stay tuned for our next session, where we'll shift gears to defense and set up alerts for detecting Mythic C2 activities! 🛡️💪

![Example Image](https://raw.githubusercontent.com/Virus192/SOC-AUTOMATION-ELK-STACK/refs/heads/main/images/photo_6017298952233272252_w.jpg)

## [Day 22: Detecting Mythic C2 Activity with Elastic Alerts and Dashboards](https://github.com/Virus192/Day-22-Detecting-Mythic-C2-Activity-with-Elastic-Alerts-and-Dashboards)

🕵️‍♂️**Day 22 of MYDFIR 30 Days SOC Challenge: Detecting Mythic C2 Activity with Elastic Alerts and Dashboards**🕵️‍♂️

Today, we focused on creating a robust detection system for Mythic C2 activity using Elastic. We set up custom alerts and built a comprehensive dashboard to visualize potential threats. Here's what we accomplished:

### Alert Creation 🚨

- Set up an alert for Mythic C2 activity based on process name and event code.
- Created a custom detection rule for specific file execution.

### Dashboard Development 📊

Built a dashboard with key visualizations:

1. **Process Creation Events (Event ID 1)**
2. **Outbound Network Connections (Event ID 3)**
3. **Windows Defender Disabled Events (Event ID 5001)**

### Key Steps 🔑

- Used Elastic's Discover feature to filter logs.
- Investigated process hashes using open-source intelligence tools.
- Created custom queries for each visualization panel.

### Tools Used 🛠️

- **Elastic Stack** (Elasticsearch, Kibana)
- **VirusTotal** for hash verification.

This hands-on exercise enhanced our ability to detect and visualize potential C2 activities in real-time. Remember, continuous monitoring and alert refinement are crucial for maintaining robust security!

Stay tuned for our next session, where we'll explore setting up a free ticketing system to manage cases and alerts effectively! 🎟️💼

![Example Image](https://raw.githubusercontent.com/Virus192/SOC-AUTOMATION-ELK-STACK/refs/heads/main/images/photo_6019550752046957237_w.jpg)

## [Day 23: Streamlining Alert Management with OS Ticket](https://github.com/Virus192/Day-23-Streamlining-Alert-Management-with-OS-Ticket)

🎟️**Day 23 of MYDFIR 30 Days SOC Challenge: Streamlining Alert Management with OS Ticket**🎟️

Today, we explored the importance of ticketing systems in managing security alerts and introduced OS Ticket as a free, open-source solution. Here's what we covered:

### Key Points 🔑
- Defined ticketing systems and their role in security operations.
- Explored benefits of using ticketing for alert management.
- Introduced OS Ticket as a free alternative to commercial solutions.

### OS Ticket Features 🛠️
- Customizable fields for tailored ticket information.
- Ticket filters for automatic routing.
- Assignment and transfer capabilities.
- Service Level Agreement (SLA) settings.

### Implementation Benefits 📊
- Improved alert tracking and documentation.
- Enhanced collaboration between teams.
- Clear audit trails for incident handling.
- Mimics the structure of a small Security Operations Center (SOC).

### Deployment Options 🖥️
- Self-hosting (on-premises) for direct control.
- Managed hosting for a hands-off approach.

### Next Steps 🚀
- Upcoming guide on setting up and configuring OS Ticket.
- Integration into existing security workflows.

This exploration of OS Ticket provides valuable insights into streamlining alert management processes. By implementing a ticketing system, we can significantly improve our incident response capabilities and overall security posture.

Stay tuned for our next session, where we'll dive into the practical setup and configuration of OS Ticket! 💪🔒

## [Day 24: Setting Up and Configuring osTicket](https://github.com/Virus192/Day-24-Setting-Up-and-Configuring-osTicket)

🎫**Day 24 of MYDFIR 30 Days SOC Challenge: Setting Up and Configuring osTicket**🎫

Today, we dove into the practical steps of deploying and configuring osTicket, an open-source ticketing system. Here's what we accomplished:

### Key Steps 🔑
- Deployed a Windows Server 2022 on Vultr.
- Set up a firewall for enhanced security (because who doesn't love a good barrier?).
- Installed XAMPP to host the web server (XAMPP: the unsung hero of local development).
- Configured XAMPP for osTicket.
- Installed and set up osTicket.
- Created and configured the MySQL database.
- Finalized osTicket configurations (not just a cakewalk, but we survived!).

### Technical Details 🛠️
- Used XAMPP (version 8.2.12) for web server hosting.
- Created firewall rules for ports 80 and 443 (because nothing says "secure" like a well-guarded entrance).
- Set up a MySQL database named **Aurora-30-Day-DB** (because every project needs a mythical reference).
- Configured file permissions for osTicket (ensuring our data is as secure as a squirrel’s stash).

### User Access 👥
- Set up end-user access through the client portal (making it as easy as pie for everyone).
- Configured admin login for staff and agent access (because someone has to keep an eye on the chaos!).

### Next Steps 🚀
- Upcoming guide on integrating osTicket with existing tech stack (because why not add another layer of complexity?).
- Plans to automate alert generation and ticket creation (so we can focus on the important stuff, like coffee breaks).

This hands-on setup of osTicket provides us with a powerful tool for managing security alerts and incidents. By implementing this ticketing system, we've taken a significant step towards professionalizing our SOC operations. 

Stay tuned for our next session, where we'll explore integrating osTicket with our existing security tools for seamless alert management! 💪🔒

![Alt text](https://raw.githubusercontent.com/Virus192/SOC-AUTOMATION-ELK-STACK/refs/heads/main/images/photo_6028481256070693563_w.jpg)

## [Day 25: Integrating OS Ticket with Elastic Stack](https://github.com/Virus192/Day-25-Integrating-OS-Ticket-with-Elastic-Stack)

🔗**Day 25 of MYDFIR 30 Days SOC Challenge: Integrating OS Ticket with Elastic Stack**🔗

Today, we focused on seamlessly integrating OS Ticket with our Elastic Stack to automate ticket creation for security alerts. Here's what we accomplished:

### Key Steps 🔑
1. Configured OS Ticket API key
2. Set up Elastic for API integration
3. Created a Webhook connector in Elastic
4. Updated OS Ticket network settings
5. Tested the integration

### Technical Details 🛠️
- Used OS Ticket's private IP for API integration
- Activated Elastic's 30-Day Free Trial for API access
- Configured Webhook connector with XML-based ticket creation
- Updated OS Ticket server's IP configuration manually

### Integration Process 🔄
- Created API key in OS Ticket admin panel
- Set up Webhook connector in Elastic Stack Management
- Configured authentication using HTTP header and API key
- Tested integration by generating a ticket from Elastic alert

### Achievements 🏆
- Successfully created a mini-SOC environment
- Automated ticket generation from Elastic alerts
- Improved incident tracking and management workflow

### Next Steps 🚀
- Upcoming guide on investigating SSH brute force alerts
- Further refinement of alert management process

This integration marks a significant milestone in our SOC automation journey, enabling seamless communication between our monitoring and ticketing systems.

Stay tuned for our next session, where we'll dive into alert investigation techniques! 💪🔍

![Alt text](https://raw.githubusercontent.com/Virus192/SOC-AUTOMATION-ELK-STACK/refs/heads/main/images/photo_6030733055884378790_w.jpg)

## [Day 26: Investigating SSH Brute Force Alerts]()

🕵️**Day 26 of MYDFIR 30 Days SOC Challenge: Investigating SSH Brute Force Alerts**🕵️

Today, we delved into the process of investigating SSH Brute Force alerts and automating our response. Here's what we covered:

### Key Investigation Steps 🔑
1. Analyzed the suspicious IP address
2. Identified affected users
3. Checked for successful login attempts
4. Investigated post-login activities (if any)

### Tools Used 🛠️
- Elastic Security dashboard
- AbuseIPDB for IP reputation check
- GreyNoise for additional IP intelligence

### Alert Automation 🔄
- Modified detection rules to send alerts to OS Ticket
- Configured Webhook action for each alert
- Set up ticket creation in OS Ticket for incoming alerts

### Ticket Management 📋
- Accessed OS Ticket Admin Panel
- Reviewed and assigned incoming alert tickets

### Key Findings 🔍
- Identified malicious IP associated with brute force attacks
- Determined affected user (root)
- No successful login attempts detected
- No post-login activity to investigate

### Next Steps 🚀
- Upcoming guide on investigating RDP Brute Force activity

This hands-on investigation of SSH Brute Force alerts has enhanced our ability to detect, analyze, and respond to potential security threats efficiently.

Stay tuned for our next session, where we'll explore RDP Brute Force detection and mitigation techniques! 💪🔒

![Alt text](path/to/image.png)
