# 🖥️ Task 7 - System Monitoring with Netdata 

## 📌 Objective
The objective of this task is to install and explore **Netdata**, a real-time monitoring tool, using a Docker container. The tool helps in visualizing system metrics such as CPU, Memory, Disk usage, and Docker containers' performance.

---

## 🐳 Netdata Setup (Docker Based)

### 🛠️ Step 1: Run Netdata Container
```bash
docker run -d \
  --name=netdata \
  -p 19999:19999 \
  --cap-add SYS_PTRACE \
  --security-opt apparmor=unconfined \
  netdata/netdata
```
---

📊 Step 2: Open Netdata Dashboard

Visit: http://localhost:19999

Example: http://13.203.194.210:19999

You’ll see a real-time dashboard with over 850+ system metrics.

---

📈 Step 3: Monitor These Metrics on Dashboard

🔍 System Metrics Monitored:

CPU Usage

Memory Usage

Disk Usage

Network Traffic

Docker Container Stats

🧪 Advanced Monitoring:

Navigate to: System → Processes → Apps → CPU/Memory/Disk

Explore:

Process utilization

Swap memory

Tasks and I/O stats

---

🔔 Step 4: Alerts and Logs

Alerts:

Click on Alerts tab (top bar)

View any warning/critical alert messages


# Check system logs
cd /var/log/netdata

ls -l

you will see the all log files

---
