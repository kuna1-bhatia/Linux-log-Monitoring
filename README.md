📁 GitHub Repository Structure
linux-log-monitoring/
│
├── README.md
├── commands.sh
├── logs/
│   └── sample.log
├── output.txt
└── screenshots/
    └── (optional terminal screenshots)

📄 README.md
# 🐧 Beginner Linux Project – Log Monitoring

This project demonstrates **Linux log monitoring**, which is a critical real-world skill for **System Administrators, DevOps Engineers, and Cloud Engineers**.

Log monitoring helps detect errors, security issues, and application problems on production servers.

---

## 📌 Project Objectives

- Monitor live logs using `tail -f`
- Search and filter errors using `grep`
- View logs efficiently using `less`
- Redirect log output to files
- Use text-processing tools like `awk`
- Understand real-world server log analysis

---

## 🛠️ Commands Used

| Command | Purpose |
|------|--------|
| `tail` | View last lines of logs |
| `grep` | Filter specific patterns |
| `less` | Read large log files |
| `cat` | Display file content |
| `awk` | Process and analyze logs |

---

## 📂 Common Log Files (Linux)

| Log File | Description |
|------|-------------|
| `/var/log/syslog` | System logs |
| `/var/log/auth.log` | Authentication logs |
| `/var/log/messages` | General messages |
| `/var/log/nginx/access.log` | Web server logs |

---

## 🚀 Steps Performed

### 1️⃣ Monitor Logs in Real-Time
```bash
sudo tail -f /var/log/syslog

2️⃣ Filter Errors Using grep
sudo grep error /var/log/syslog


Case-insensitive search:

sudo grep -i error /var/log/syslog

3️⃣ Save Filtered Logs to File
sudo grep error /var/log/syslog > error_logs.txt


Append output:

sudo grep warning /var/log/syslog >> error_logs.txt

4️⃣ View Logs Using less
less /var/log/syslog


🧠 Why This Project Is Important?

📌 Used daily on production servers
📌 Helps detect system failures early
📌 Required for DevOps & Cloud roles
📌 Strong interview talking point

🎯 Learning Outcome

✔ Real-time log monitoring
✔ Error detection & filtering
✔ File redirection & piping
✔ Production-level Linux skill

🧑‍💻 Author

Kunal Bhatia
Linux | DevOps | Cloud Learner 🚀

⭐ GitHub Tip

Star ⭐ the repository if this project helped you!


---

# 📜 `commands.sh`

```bash
#!/bin/bash

# Monitor logs
sudo tail -f /var/log/syslog

# Filter errors
sudo grep error /var/log/syslog

# Save output to file
sudo grep error /var/log/syslog > error_logs.txt



Make executable:

chmod +x commands.sh

📝 logs/sample.log (Optional Demo Log)
Jan 10 12:20 systemd Started service
Jan 10 12:22 systemd Error starting service
Jan 10 12:25 sshd Failed password for user
