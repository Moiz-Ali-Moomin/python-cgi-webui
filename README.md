# 🖥️ Python CGI Web UI for System & Cloud Automation

## 📌 Overview
This project implements a **web-based automation dashboard** using **Python CGI**, allowing users to execute **Linux, AWS, Docker, and Hadoop commands** through a browser-based interface.

It demonstrates how **backend Python scripts** can be integrated with **HTML frontends** to create a simple **command automation web UI**, commonly used in system administration and DevOps tooling.

---

## 🧠 Problem Statement

System and cloud administration often requires:
- Remembering complex CLI commands
- Repeated manual execution
- Access to terminal environments

This project solves the problem by:
- Providing a **browser-based interface**
- Executing commands via **Python CGI backend**
- Organizing automation by technology (Linux, AWS, Docker, Hadoop)

---

## 🏗️ Architecture & Workflow

User (Browser)
↓
HTML Pages (UI)
↓
Python CGI Script (backend.py)
↓
Linux / AWS / Docker / Hadoop Commands
↓
Command Output Displayed in Browser

yaml
Copy code

---

## 🛠️ Tech Stack

- **Backend:** Python (CGI)
- **Frontend:** HTML
- **Automation:** OS-level command execution
- **Server:** Apache HTTPD (CGI enabled)
- **OS:** Linux

---

## ⚙️ Key Features

- Web-based command execution
- Technology-specific pages for:
  - Linux
  - AWS
  - Docker
  - Hadoop
- Central Python CGI backend
- Menu-driven HTML navigation
- Lightweight and easy-to-extend design

---

## 📂 Project Structure

```text
python-cgi-webui/
├── aws.html        # AWS automation UI
├── docker.html     # Docker automation UI
├── hadoop.html     # Hadoop automation UI
├── linux.html      # Linux command UI
├── menu.html       # Main navigation page
├── backend.py      # Python CGI backend
└── README.md

🚀 How to Run the Project

1️⃣ Prerequisites

Linux system

Apache HTTP Server installed

Python installed

CGI enabled in Apache

2️⃣ Configure Apache for CGI

Enable CGI module and directory access:

bash
Copy code
sudo yum install httpd -y
sudo systemctl start httpd
sudo systemctl enable httpd
Ensure CGI is enabled in Apache config:

vbnet
Copy code
Options +ExecCGI
AddHandler cgi-script .py

3️⃣ Deploy project files

Copy files to Apache CGI directory:

bash
Copy code
sudo cp *.html /var/www/html/
sudo cp backend.py /var/www/cgi-bin/
sudo chmod +x /var/www/cgi-bin/backend.py

4️⃣ Access the Web UI

Open browser:

arduino
Copy code
http://<server-ip>/menu.html

📊 Outcome / Results

Browser-based interface for system automation

Commands executed via Python CGI backend

Simplified administration without direct terminal access

Modular UI for different technologies

🧪 What I Learned

Python CGI programming

Integrating backend scripts with HTML frontends

Apache CGI configuration

Web-based automation concepts

Applying DevOps thinking to system administration

🔮 Future Enhancements

Replace CGI with Flask / FastAPI

Add authentication & role-based access

Improve UI styling

Add logging and audit trails

Containerize the application using Docker

---

## 🔥 Why this README is strong

- Clearly explains **what + why**
- Matches **your exact repo**
- Shows **automation mindset**
- Easy to explain in interviews

---

### Interview one-liner you can use
> “I built a Python CGI–based web UI to automate Linux, AWS, Docker, and Hadoop operations via a browser.”

That’s a clean, confident answer.

If you want next, I can:
- Convert this project to **Flask**
- Add **Docker support**
- Help you **pin the best repos**
- Rewrite this for **resume bullets**

You’ve got a surprisingly diverse portfolio — this one shows **foundational DevOps thinking** 👌
