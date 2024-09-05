# ELK SOC Automation - 30 Days SOC Challenge
 ELK Stack SOC automation using Fleet and OS Ticketing Server

## Day ONE: Logical Diagram

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
## Day 3: Building a Secure Elasticsearch Deployment

🌟 **Day Three of MYDFIR SOC Challenge: Building a Secure Elasticsearch Deployment** 🌟  
Today was all about diving deep into the world of Elasticsearch! 🎯 As part of the 30 Days SOC Challenge, I set up and secured an Elasticsearch instance.

### What’s on the Plate?
- Installed **Elasticsearch** on a robust Ubuntu 22.04 LTS environment. 🐧
- Ensured a secure deployment by implementing a well-configured firewall. 🔒
- Deployed within a VPC 2.0 on Vultr for enhanced network security. 🌐

### Key Takeaways:
- **Ubuntu 22.04 LTS** provides a stable and secure foundation for hosting Elasticsearch.
- A secured **firewall setup** is non-negotiable—it protects our data and services.
- Leveraging **VPC 2.0** in Vultr adds network segmentation and security.

FREE $300 Cloud Credit (Vultr): [link](https://lnkd.in/drVeaA5s)

---

## Day 4: Elasticsearch Security Configuration

### Security autoconfiguration information:

- Authentication and authorization are enabled.
- TLS for the transport and HTTP layers is enabled and configured.
  
The generated password for the `elastic` built-in superuser is: `OK6A_2wP9DZql=hYsc1M`.

If this node should join an existing cluster, you can reconfigure this with:
```bash
/usr/share/elasticsearch/bin/elasticsearch-reconfigure-node --enrollment-token <token-here>
