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

## [Day 6: Deploying a Windows Server on Vultr Cloud](https://github.com/Virus192/Day-6-Deploying-a-Windows-Server-on-Vultr-Cloud)

 🚀 **Day 6 of MYDFIR 30 Days SOC Challenge: Deploying a Windows Server on Vultr Cloud** 🚀

Today’s focus was on deploying a Windows Server and making it publicly accessible. We moved both our Windows and Ubuntu Servers out of VPC 2.0 to expose them to the internet. Here’s a step-by-step breakdown of how I accomplished this task.

## Quick Steps

1. **Login to Vultr Cloud:** Start by logging into your Vultr Cloud account and clicking on the **Deploy +** button.
2. **Choose Server Type:** For this deployment, I selected **Cloud Compute — Shared CPU**, a cost-effective solution for light processing tasks.
3. **Select Plan:** I opted for the **55GB SSD storage, 1 vCPU, and 2GB memory** plan, providing an ideal balance of cost and performance.
4. **Deploy:** After selecting the configuration, clicking **Deploy Now** begins the installation, which completes in around 5-7 minutes.
5. **Access Server:** Once deployed, Vultr provides the credentials to log into the Windows Server, which is now publicly accessible.

## Why This Matters

Deploying a Windows Server on Vultr Cloud is quick and easy, making it a great option for creating publicly available servers while keeping costs low. Looking forward to more challenges ahead!

![insert image here](image.jpg)

## [Day 7: Introduction to Fleet Server and Elastic Agent](https://github.com/Virus192/Day-6-Deploying-a-Windows-Server-on-Vultr-Cloud)

 🌟 **Day 7 of MYDFIR 30 Days SOC Challenge: Exploring Fleet Server and Elastic Agent** 🌟

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

![insert image here](image.jpg)

