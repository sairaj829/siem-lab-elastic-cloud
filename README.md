# SIEM Lab Using Elastic Cloud on Kali Linux  

A hands-on cybersecurity project where I deployed a SIEM (Security Information and Event Management) lab using Elastic Cloud on Kali Linux, monitored system logs, created alerts for security events, and tested detection by simulating an SSH brute-force attack. 

## Project Overview  
This project demonstrates how **Elastic Stack (Elasticsearch, Kibana, Logstash, and Filebeat)** can be used as a **SIEM solution** to monitor security logs, detect threats, and respond to incidents in real-time.  

### Key Objectives:  
✔️ Deploy **SIEM** on **Elastic Cloud** to monitor security logs.  
✔️ Set up **Filebeat** on Kali Linux to collect and forward logs.  
✔️ Create **custom detection rules** and alerts in Kibana.  
✔️ Simulate an **SSH brute-force attack** to test the alerting system.  
✔️ Learn how to **analyze and visualize security incidents**.  

## 🛠 Tech Stack  
- **Elastic Cloud** – Cloud-based SIEM platform.  
- **Kali Linux** – Security-focused Linux distribution.  
- **Elasticsearch** – Log storage and indexing.  
- **Kibana** – Data visualization and security analytics.  
- **Filebeat** – Log shipper for forwarding logs.  
- **Logstash** – Optional for advanced log processing.  
- **Hydra** – Used for SSH brute-force attack simulation.  

##  Project Setup & Configuration  

### 1️⃣ Deploying SIEM on Elastic Cloud  
1. **Sign up for Elastic Cloud** at [elastic.co](https://www.elastic.co/).  
2. **Create a new deployment** and select **Elastic Stack** (Elasticsearch + Kibana).  
3. Copy your **Elasticsearch endpoint**, **Kibana URL**, and **credentials**.  
4. Log in to **Kibana** and navigate to **Security → Detections & Rules** to manage alerts.  

### 2️⃣ Installing and Configuring Filebeat on Kali Linux  
1. Download and install Filebeat:  
   ```bash
   curl -L -O https://artifacts.elastic.co/downloads/beats/filebeat/filebeat-8.x.x-amd64.deb  
   sudo dpkg -i filebeat-8.x.x-amd64.deb  

