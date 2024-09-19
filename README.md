# 🔒 **Linux Privilege Escalation Tools**

## 📝 **Overview**
This repository provides a curated collection of tools to assist security professionals in identifying privilege escalation opportunities within Linux environments. Each tool serves a distinct purpose, from system enumeration to real-time process monitoring, helping detect misconfigurations that could allow unauthorized access.

### 📦 **Included Tools**:
1. **linpeas.sh**
2. **les.sh** (Linux Exploit Suggester)
3. **LinEnum** (Linux Enumeration)
4. **linuxprivchecker.py**
5. **pspy64**

---

## 📑 **Table of Contents**

- [🔍 linpeas.sh](#-linpeassh)
- [🛡️ les.sh](#-lessh)
- [📋 LinEnum](#-linenum)
- [🐍 linuxprivchecker.py](#-linuxprivcheckerpy)
- [🖥️ pspy64](#pspy64)

---

## 🛠 **linpeas.sh**

### 🔍 **Description**
`linpeas.sh` is a comprehensive shell script designed to search for potential privilege escalation paths on Linux systems. It identifies common misconfigurations and vulnerabilities that attackers can exploit to gain elevated privileges.

### 🌟 **Key Features**
- In-depth system enumeration.
- Identifies weak file permissions, vulnerable services, and other security risks.
- Provides colorful and easy-to-interpret output.

### 📊 **Output Interpretation**
- **Kernel vulnerabilities:** Lists any known kernel issues.
- **Insecure file permissions:** Highlights files and directories with weak permissions.
- **SUID binaries:** Displays SUID binaries that may be exploitable.
- **Writable directories:** Identifies directories writable by unauthorized users.

---

## 🛡️ **lessh**

### 🔍 **Description**
`les.sh` (Linux Exploit Suggester) is a lightweight script that scans a system for known vulnerabilities based on its kernel and distribution version. It's a quick way to assess security risks on Linux systems.

### 🌟 **Key Features**
- Fast, lightweight, and easy-to-use.
- Suggests exploits based on the system's kernel and software packages.

### 📊 **Output Interpretation**
- Outputs a list of known vulnerabilities and suggested exploits based on the kernel version and installed packages.

---

## 📋 **LinEnum**

### 🔍 **Description**
`LinEnum` is an advanced script that performs an extensive assessment of Linux systems, helping identify potential privilege escalation vectors by systematically checking the system's configuration.

### 🌟 **Key Features**
- Comprehensive enumeration of users, groups, and running processes.
- Identifies SUID files, writable directories, and services running as root.
- Generates detailed and easy-to-understand reports.

### 📊 **Output Interpretation**
- Provides a thorough report of system configurations, security settings, and misconfigurations that could be exploited.

---

## 🐍 **linuxprivchecker.py**

### 🔍 **Description**
`linuxprivchecker.py` is a Python-based script for auditing Linux systems to identify potential privilege escalation opportunities. It checks for weak file permissions, cron jobs, and misconfigured services.

### 🌟 **Key Features**
- Identifies SUID files, cron jobs, and world-writable directories.
- Detects misconfigured services and weak system settings.

### 📊 **Output Interpretation**
- Provides a list of actionable items such as misconfigured services or improperly set file permissions that may allow privilege escalation.

---

## 🖥️ **pspy64**

### 🔍 **Description**
`pspy64` is a real-time process monitoring tool that allows you to observe processes executed by other users (including root) without elevated privileges. This tool is especially useful for detecting cron jobs or hidden processes that could be exploited.

### 🌟 **Key Features**
- Monitors system process executions in real-time.
- Requires no root permissions for execution.
- Helps uncover hidden or low-privilege processes that could lead to system vulnerabilities.

### 📊 **Output Interpretation**
- Provides a real-time log of system processes, highlighting potential security risks such as cron jobs or user-executed commands.

---

## ⚙️ **Usage**

```bash
# Download linpeas.sh
git clone https://github.com/vishuchauhan27/linpeas.sh
```

# Give execution permission
```bash
chmod +x linpeas.sh
```

# Run linpeas.sh
```bash
./linpeas.sh
```
