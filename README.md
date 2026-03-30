# 🛠️ Open Source Audit Toolkit

> *"Built on giants. Paying it forward."*

A powerful collection of Bash scripts for auditing, analyzing, and celebrating open-source software on Linux systems. Whether you're inspecting packages, scanning permissions, digging through logs, or writing your FOSS manifesto — this toolkit has you covered.

---

## 📖 Table of Contents

- [Overview](#-overview)
- [Scripts](#-scripts)
  - [1. System Identity Report](#1-system-identity-report)
  - [2. FOSS Package Inspector](#2-foss-package-inspector)
  - [3. Disk & Permission Auditor](#3-disk--permission-auditor)
  - [4. Log File Analyzer](#4-log-file-analyzer)
  - [5. Open Source Manifesto Generator](#5-open-source-manifesto-generator)
- [Requirements](#-requirements)
- [Installation](#-installation)
- [Quick Start](#-quick-start)
- [Philosophy](#-philosophy)
- [License](#-license)
- [Author](#-author)

---

## 🌐 Overview

This project contains **five specialized Bash scripts** designed to help you understand and audit your Linux system from an open-source perspective. Each script focuses on a different aspect of system analysis rooted in **FOSS (Free and Open Source Software)** principles.

---

## 📜 Scripts

---

### 1. System Identity Report

**File:** `script.sh`

Generates a comprehensive system identity report — kernel version, distribution info, user details, uptime, and licensing highlights.

**✨ Features:**
- Displays current kernel version and Linux distribution
- Shows logged-in user and home directory
- Reports system uptime and current date/time
- Highlights **GPL v2** licensing information

**▶️ Usage:**
```bash
bash script.sh
```

**📋 Output includes:**
- Student name and project information
- Linux distribution and kernel version
- Current user and home directory path
- System uptime
- OS licensing details (GPL v2)

---

### 2. FOSS Package Inspector

**File:** `script2.sh`

Inspects installed FOSS packages and provides philosophical context about their importance in the open-source ecosystem.

**✨ Features:**
- Auto-detects package manager (RPM or DEB-based)
- Queries running kernel package information
- Provides contextual info about major FOSS projects
- Works across different Linux distributions

**▶️ Usage:**
```bash
bash script2.sh
```

**📦 Supported Packages:**

| Package | Description |
|--------|-------------|
| Linux Kernel | Core of the OS |
| Apache / httpd | Web server |
| MySQL / MariaDB | Database engine |
| Python | Scripting language |
| Git | Version control |
| And more... | |

---

### 3. Disk & Permission Auditor

**File:** `script3.sh`

Audits critical system directories for permissions, ownership, and disk usage — essential for any security-conscious sysadmin.

**✨ Features:**
- Scans multiple critical system directories
- Reports permissions, owner, group, and size for each
- Checks kernel config file existence and permissions
- Handles missing directories gracefully

**▶️ Usage:**
```bash
bash script3.sh
```

**📁 Audited Directories:**

| Directory | Purpose |
|-----------|---------|
| `/etc` | System configuration |
| `/var/log` | System logs |
| `/home` | User home directories |
| `/usr/bin` | User binaries |
| `/tmp` | Temporary files |
| `/boot` | Boot files and kernel |
| `/lib` | System libraries |

---

### 4. Log File Analyzer

**File:** `script4.sh`

Analyzes log files for specific keywords, providing match counts and the most recent matching entries.

**✨ Features:**
- Case-insensitive keyword search
- Counts total matches
- Displays the last 5 matching lines
- Handles empty/missing files with retry logic
- Defaults to `"error"` if no keyword specified

**▶️ Usage:**
```bash
bash script4.sh <logfile> [keyword]
```

**💡 Examples:**
```bash
# Search for errors in syslog
bash script4.sh /var/log/syslog error

# Search for warnings in auth.log
bash script4.sh /var/log/auth.log warning

# Search for failed login attempts
bash script4.sh /var/log/auth.log failed
```

**📌 Parameters:**

| Parameter | Required | Default | Description |
|-----------|----------|---------|-------------|
| `logfile` | ✅ Yes | — | Path to the log file |
| `keyword` | ❌ No | `error` | Term to search for |

---

### 5. Open Source Manifesto Generator

**File:** `script5.sh`

An interactive script that generates a personalized open-source manifesto based on your values and vision.

**✨ Features:**
- Interactive questionnaire about open-source values
- Generates a timestamped manifesto file
- Creates unique output files to prevent overwrites
- Celebrates FOSS philosophy and community contribution

**▶️ Usage:**
```bash
bash script5.sh
```

**💬 Interactive Prompts:**
1. *Name one open-source tool you use every day*
2. *In one word, what does freedom mean to you?*
3. *Name one thing you would build and share freely*

**📄 Output:**
- Creates `manifesto_<username>_<timestamp>.txt`
- Displays your personalized manifesto on screen

---

## ⚙️ Requirements

- Linux-based operating system
- Bash shell (version 4.0 or higher recommended)
- Standard Unix utilities: `uname`, `whoami`, `uptime`, `date`, `grep`, `awk`, `du`, `ls`
- Package manager: `rpm` or `dpkg` *(for `script2.sh`)*
- Appropriate permissions to read system directories and log files

---

## 📥 Installation

**1. Clone or download this repository:**
```bash
git clone https://github.com/your-username/open-source-audit-toolkit.git
cd open-source-audit-toolkit
```

**2. Make all scripts executable:**
```bash
chmod +x script.sh script2.sh script3.sh script4.sh script5.sh
```

---

## 🚀 Quick Start

Run all scripts in sequence to get a full system audit:

```bash
bash script.sh        # System Identity Report
bash script2.sh       # FOSS Package Inspector
bash script3.sh       # Disk & Permission Auditor
bash script4.sh /var/log/syslog   # Log File Analyzer
bash script5.sh       # Manifesto Generator
```

---

## 💡 Philosophy

This toolkit embodies the four essential freedoms of Free and Open Source Software:

| Freedom | Description |
|---------|-------------|
| 🔍 **Study** | All scripts are readable and well-commented |
| ✏️ **Modify** | Adapt these scripts to your specific needs |
| 📤 **Share** | Distribute and improve these tools freely |
| 🤝 **Community** | Built on the shoulders of open-source giants |

---

## 📄 License

This project celebrates open-source software and the **GPL v2 license** under which the Linux kernel is distributed. The scripts are provided as educational tools for understanding and auditing FOSS systems.

---

## 👤 Author

**Adarsh Kumar**
*Open Source Audit Project*

> *"Built on giants. Paying it forward."*

---

<div align="center">
  ⭐ If you found this useful, give it a star and share it with the community!
</div>
