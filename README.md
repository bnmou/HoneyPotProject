# **Honeypot Project: Deploying and Analyzing TPot in a Cloud Environment**

## **Overview**
This project highlights the deployment and use of the TPot multi-honeypot platform on a cloud-based Ubuntu server. The goal is to showcase my ability to set up, configure, and analyze honeypot data to understand malicious activity. By utilizing tools such as Kibana, Talos Intelligence, and TPot's dashboards, this project demonstrates my skills in network monitoring, threat intelligence, and incident analysis.

## **Project Objectives**
- Deploy a secure Ubuntu cloud server to host TPot.
- Install and configure TPot to monitor and capture attack traffic.
- Analyze incoming attack data using Kibana and other visualization tools.
- Investigate attackers' IP addresses and reputations using Talos Intelligence.
- Leverage insights from honeypot-specific dashboards like Honeytrap, Suricata, and Cowrie.

---

## **Project Steps**

### **1. Setting Up an Ubuntu Cloud Server**
I started by provisioning an Ubuntu cloud server on Vultr. The process included selecting the server type, configuring resources (CPU, memory, and storage), and setting up SSH access for secure administration. Ubuntu was chosen for its lightweight architecture and compatibility with TPot.

- **Key Skills Demonstrated:** Cloud provisioning, server configuration, secure access via SSH.
- **Challenges Overcome:** Configuring server firewalls to balance security with honeypot accessibility.

*Screenshot:* Setting up the Ubuntu cloud server in Vultr's interface.
![setting up ubuntu cloud server with vultr](https://github.com/user-attachments/assets/1a1b3975-3c31-4cc5-8e20-4c4347fff5eb)

---

### **2. Installing TPot**
Once the server was set up, I installed TPot using the TPotCE (Community Edition) repository. This included preparing the server by installing prerequisites, downloading the TPot installation script, and running the setup. The script automates the deployment of multiple honeypot systems, making it ideal for comprehensive threat monitoring.

- **Key Skills Demonstrated:** Linux command-line usage, installation of complex software stacks.
- **Challenges Overcome:** Ensuring all dependencies (Docker, Compose, etc.) were correctly installed.

*Screenshot:* Terminal output during TPot installation.
![installing tpot onto our ubuntu server](https://github.com/user-attachments/assets/d8015265-e68a-47dd-b2e3-05e36fda8773)

---

### **3. Successfully Accessing TPot**
After installation, I accessed TPot's web interface using the server's IP address on port `64297`. This interface provides centralized access to dashboards, logs, and attack analytics. Authentication ensured the system remained secure while providing insights into activity.

- **Key Skills Demonstrated:** Web interface navigation, user authentication configuration.
- **Challenges Overcome:** Configuring and verifying network settings to ensure accessibility.

*Screenshot:* Successful login to the TPot web interface.
![successfully logged into tpot](https://github.com/user-attachments/assets/a0f1a86b-d5c6-4298-a6f6-318a9f0844a6)

---

### **4. Configuring Firewall for Open Access**
To attract attackers, I adjusted the cloud provider's firewall settings to allow unrestricted inbound traffic to the server. This configuration is vital for collecting diverse attack data but requires caution to avoid exposing other services.

- **Key Skills Demonstrated:** Network security and firewall configuration.
- **Challenges Overcome:** Ensuring only the honeypot services were exposed to attackers.

*Screenshot:* Cloud service firewall configuration allowing unrestricted inbound access.
![configuring firewall on cloud service to be open to all attackers ](https://github.com/user-attachments/assets/84702e4b-ca86-43ce-ba92-365138c39216)

---

### **5. Observing the Attack Map**
Within minutes of deployment, the TPot attack map began displaying malicious traffic. The map provided a visual representation of attackers' geographic locations, revealing the global nature of cyber threats.

- **Key Skills Demonstrated:** Monitoring and visualizing real-time attack traffic.
- **Challenges Overcome:** Understanding and interpreting attack influx patterns.

*Screenshot:* TPot attack map showcasing an influx of attackers.
![attack map showing large influx of attackers within minutes of opening network](https://github.com/user-attachments/assets/8ed65931-c505-409c-a2ea-ef37a973d4ca)

---

### **6. Analyzing Logs in Kibana**
Kibana's Honeytrap dashboard allowed me to analyze logs from a specific honeypot service. I explored data such as connection attempts, source IPs, and interaction types, gaining a detailed understanding of the attackers' actions.

- **Key Skills Demonstrated:** Log analysis, using SIEM tools for data visualization.
- **Challenges Overcome:** Filtering through large datasets to identify meaningful patterns.

*Screenshot:* Kibana dashboard displaying Honeytrap logs.
![Kibana tool showing dashboard for honeytrap logs ](https://github.com/user-attachments/assets/3796429f-c3d1-4693-b4d5-0792600abb37)

---

### **7. Filtering Data for Deeper Analysis**
Using Kibana's filtering capabilities, I narrowed down attack data by specific parameters, such as source IPs or event types. This helped identify trends and anomalies, providing actionable intelligence.

- **Key Skills Demonstrated:** Advanced filtering techniques, data interpretation.
- **Challenges Overcome:** Extracting relevant insights from a high volume of logs.

*Screenshot:* Kibana filter view for detailed log analysis.
![more detailed view of the dashboard allows us to filter infomration onto an organized view](https://github.com/user-attachments/assets/a7711f0d-34cb-4a3b-bee8-cc5106cbaabf)

---

### **8. Investigating IPs with Talos Intelligence**
To gather more details about attackers, I performed IP lookups using Talos Intelligence. This step provided information on attackers' geolocations, reputations, and historical activity, enriching my understanding of the threats.

- **Key Skills Demonstrated:** Threat intelligence research, leveraging external tools.
- **Challenges Overcome:** Correlating data from multiple sources to create a complete picture.

*Screenshot:* Talos Intelligence results for an attacker’s IP.
![individual IP lookup with Talos Intelligence](https://github.com/user-attachments/assets/64c212b1-9198-4252-ad28-3e43b64c9444)

---

### **9. Exploring Other Honeypot Dashboards: Suricata**
The Suricata dashboard offered insights into network traffic patterns and malicious payloads detected. This added a layer of depth to the analysis by revealing more details about attackers' methods.

- **Key Skills Demonstrated:** Analyzing network activity, understanding intrusion detection systems.
- **Challenges Overcome:** Interpreting complex network data for actionable insights.

*Screenshot:* Suricata dashboard with detailed network activity logs.
![example of other honeypot dashboards like Suricata giving more info](https://github.com/user-attachments/assets/f64da1b1-20f5-4c48-9832-5b255e2ed5f7)

---

### **10. Exploring Other Honeypot Dashboards: Cowrie**
Cowrie, a honeypot emulating SSH and Telnet services, logged detailed interactions such as login attempts and executed commands. This highlighted how attackers interact with exposed systems.

- **Key Skills Demonstrated:** Behavioral analysis of attackers, analyzing SSH/Telnet-based logs.
- **Challenges Overcome:** Differentiating between real and automated attack interactions.

*Screenshot:* Cowrie dashboard highlighting SSH-based interactions.
![example of other honeypot dashboards like Cowrie giving more insight ](https://github.com/user-attachments/assets/046e5660-b828-4c2d-9459-6e7f56374ad2)

---

## **Conclusion**
This project underscores the importance of honeypots in understanding malicious activity and gathering threat intelligence. By deploying and analyzing TPot, I gained valuable insights into attack patterns and enhanced my skills in cybersecurity operations. The hands-on experience has greatly strengthened my confidence and capabilities in blue team operations especially in the Security Operations Center environment. 
