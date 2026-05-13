# 🚨 Real-Time System Monitoring & Alerting Platform

A complete real-time Linux monitoring solution built using:

- Prometheus
- Grafana
- Alertmanager
- Node Exporter
- Docker Compose
- Telegram Bot Notifications

The system continuously monitors CPU usage, memory usage, and CPU temperature, while sending instant Telegram alerts whenever thresholds are exceeded.

---

# ✨ Features

✅ Real-time Linux system monitoring  
✅ Grafana visualization dashboards  
✅ Prometheus metrics collection  
✅ Telegram alert notifications  
✅ CPU, RAM, and temperature monitoring  
✅ Dockerized deployment  
✅ Alertmanager integration  
✅ Custom alert rules  
✅ Beginner-friendly DevOps project  

---

# 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| Prometheus | Metrics collection |
| Grafana | Visualization dashboards |
| Alertmanager | Alert handling |
| Node Exporter | Linux system metrics |
| Docker | Containerization |
| Docker Compose | Service orchestration |
| Telegram Bot API | Instant notifications |

---

# 📂 Project Structure

```bash
.
├── docker-compose.yml
├── prometheus.yml
├── alerts.yml
├── alertmanager.yml
├── screenshots/
└── README.md
```

---

# 📸 Project Screenshots

---

## 🔹 Prometheus Alerts Dashboard

Shows alert states including firing and inactive alerts.

![Prometheus Alerts](screenshots/alerts-firing.png)

---

## 🔹 Alertmanager Dashboard

Displays grouped alerts routed through Alertmanager.

![Alertmanager](screenshots/alertmanager-dashboard.png)

---

## 🔹 Telegram Alert Notifications

Real-time alert notifications delivered directly to Telegram.

![Telegram Alerts](screenshots/telegram-alerts.png)

---

## 🔹 Grafana Monitoring Dashboard

Interactive Grafana dashboard visualizing CPU, memory, network, and disk metrics.

![Grafana Dashboard](screenshots/grafana-dashboard.png)

---

# ⚙️ Setup Instructions

## 1️⃣ Clone Repository

```bash
git clone https://github.com/YOUR_USERNAME/real-time-system-monitoring.git

cd real-time-system-monitoring
```

---

## 2️⃣ Install Docker & Docker Compose

Ubuntu/Debian:

```bash
sudo apt update

sudo apt install docker.io docker-compose -y
```

---

## 3️⃣ Start Monitoring Stack

```bash
docker compose up -d
```

---

# 🌐 Service URLs

| Service | URL |
|---|---|
| Prometheus | http://localhost:9090 |
| Alertmanager | http://localhost:9093 |
| Grafana | http://localhost:3000 |

---

# 📊 Grafana Dashboard

Import Node Exporter Dashboard:

Dashboard ID:

```text
1860
```

Default Login:

```text
Username: admin
Password: admin
```

---

# 🤖 Telegram Bot Setup

## Create Telegram Bot

1. Open Telegram
2. Search for `@BotFather`
3. Run:

```text
/newbot
```

4. Copy your bot token

---

## Get Telegram Chat ID

Send a message to your bot.

Then open:

```text
https://api.telegram.org/bot<YOUR_BOT_TOKEN>/getUpdates
```

Copy your `chat_id`.

---

## Configure alertmanager.yml

```yaml
bot_token: 'YOUR_BOT_TOKEN'
chat_id: YOUR_CHAT_ID
```

---

# 🚨 Current Alert Rules

| Alert | Trigger Condition |
|---|---|
| High CPU Usage | CPU > 70% |
| High Memory Usage | RAM > 80% |
| High CPU Temperature | Temp > 85°C |

---

# 🧪 Testing Alerts

## CPU Stress Test

```bash
stress --cpu 8 --timeout 60
```

---

## Memory Stress Test

```bash
stress --vm 2 --vm-bytes 2G --timeout 60
```

---

# 📲 Example Telegram Alert

```text
🚨 ALERT 🚨

Alert: HighCPUUsage
Severity: warning

Summary:
High CPU Usage Detected

Description:
CPU usage is above 70%
```

---

# 👨‍💻 Who Can Use This?

This project is useful for:

- DevOps Engineers
- Linux Administrators
- Cloud Engineers
- SRE Engineers
- Students learning monitoring systems
- Home lab users
- Raspberry Pi users
- Small server infrastructure monitoring

---

# 💡 Real-World Use Cases

- Server health monitoring
- Production alerting systems
- Infrastructure monitoring
- Cloud VM monitoring
- Self-hosted monitoring stacks
- Linux performance monitoring
- Homelab monitoring

---

# 🚀 Future Improvements

- AWS EC2 deployment
- Kubernetes monitoring
- Email notifications
- Slack/Discord integrations
- Disk usage alerts
- Uptime monitoring
- Multi-server monitoring

---

# 📚 Learning Outcomes

Through this project, I learned:

- Docker container orchestration
- Infrastructure monitoring
- Prometheus alert rules
- Grafana dashboards
- Alertmanager configuration
- Linux metrics collection
- Telegram API integration
- YAML configuration
- DevOps fundamentals

---

# 💼 Resume Value

This project demonstrates practical experience in:

- DevOps
- Docker
- Linux
- Monitoring & Alerting
- Infrastructure Automation
- Observability
- System Administration

---

# 🔒 Important Security Note

Before pushing to GitHub:

❌ NEVER upload:

- Telegram Bot Token
- Chat ID
- API secrets

Replace them with:

```yaml
bot_token: 'YOUR_BOT_TOKEN'
chat_id: YOUR_CHAT_ID
```

---

# ⭐ GitHub Topics

```text
prometheus
grafana
docker
alertmanager
node-exporter
devops
linux-monitoring
telegram-bot
system-monitoring
observability
```

---

# 📄 License

MIT License

---

# ⭐ Support

If you found this useful, give the repository a star ⭐
