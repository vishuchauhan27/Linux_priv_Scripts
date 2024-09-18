# 🔒 Linux Privilege Escalation Tools

## 📝 Overview

This repository includes a collection of powerful tools designed to aid in identifying potential privilege escalation vectors in Linux environments. Each tool serves a unique purpose, from system enumeration to real-time process monitoring, helping security professionals find misconfigurations that could lead to unauthorized access.

### Included Tools:

1. **linpeas.sh**
2. **les.sh**
3. **LinEnum**
4. **linuxprivchecker.py**
5. **pspy64**

---

## 📑 Table of Contents

- [linpeas.sh](#linpeassh)
- [les.sh](#lessh)
- [LinEnum](#linenum)
- [linuxprivchecker.py](#linuxprivcheckerpy)
- [pspy64](#pspy64)

---

## 🛠 linpeas.sh

### Description
`linpeas.sh` is an advanced shell script that searches for potential privilege escalation paths on Linux systems. It performs an in-depth check for common misconfigurations and exploits that could be leveraged to gain higher privileges.

### Key Features
- Comprehensive system enumeration.
- Identifies weak file permissions, vulnerable services, and potential security risks.
- Outputs colorful and easy-to-interpret results.

### Output Interpretation
The script will display a detailed summary of findings such as:

- Kernel vulnerabilities.
- Insecure file permissions.
- SUID binaries.
- Writable directories and much more.
  
### Description
les.sh (Linux Exploit Suggester) is a lightweight script that enumerates the system for known vulnerabilities based on kernel and distribution information. It provides a quick way to check for security misconfigurations.

- Key Features
- Fast and easy-to-use.
- Provides quick recommendations based on the system’s kernel and packages.
  
### Output Interpretation
The script outputs a list of known vulnerabilities based on the kernel version and potential exploits that can be used to escalate privileges.
### escription
LinEnum performs an extensive privilege escalation assessment on Linux machines. It is ideal for obtaining a complete overview of system security, listing misconfigurations, and discovering exploitable flaws.

- Key Features
- Systematic enumeration of user, group, and process information.
- Highlights SUID files, writable directories, and services running as root.
- Easy-to-understand report generation.
  
### Output Interpretation
LinEnum produces a comprehensive report detailing system configurations, security settings, and potential privilege escalation paths.
Description
linuxprivchecker.py is a Python-based tool for auditing a Linux system to identify privilege escalation opportunities. The script is particularly useful for system administrators and penetration testers.

- Key Features
- Checks SUID files, cron jobs, and system-wide writable directories.
- Detects weak file permissions and misconfigured services.
  
 ### Output Interpretation
 The script outputs actionable suggestions for privilege escalation, highlighting weak areas like improperly configured services and exploitable system settings.

 ### Description
pspy64 is a real-time process monitor that allows you to see commands executed by other users (including root) without needing elevated privileges. This tool is excellent for monitoring cron jobs, services, or other processes that could be leveraged to escalate privileges.

- Key Features
- Monitors and captures system process executions.
- No root permissions required for execution.
- Detects hidden or low-privilege processes that can lead to system vulnerabilities.
  ### Output Interpretation
pspy64 will output a real-time log of system processes, helping identify exploitable commands or cron jobs run by privileged users.
### Usage
```bash
# Download linpeas.sh
curl -Lo linpeas.sh https://github.com/carlospolop/PEASS-ng/releases/download/refs/tags/20230918-linpeas-ng-release/linpeas.sh

# Give execution permission
chmod +x linpeas.sh

# Run linpeas.sh
./linpeas.sh

# Download les.sh
curl -Lo les.sh https://raw.githubusercontent.com/mzet-/linux-exploit-suggester/master/les.sh

# Give execution permission
chmod +x les.sh

# Run les.sh
./les.sh
# Download LinEnum
curl -Lo LinEnum.sh https://raw.githubusercontent.com/rebootuser/LinEnum/master/LinEnum.sh

# Give execution permission
chmod +x LinEnum.sh

# Run LinEnum with report generation
./LinEnum.sh -r report.txt
# Download linuxprivchecker.py
curl -Lo linuxprivchecker.py https://raw.githubusercontent.com/sleventyeleven/linuxprivchecker/master/linuxprivchecker.py

# Run the script
python linuxprivchecker.py
# Download pspy64
curl -Lo pspy64 https://github.com/DominicBreuker/pspy/releases/download/v1.2.1/pspy64

# Give execution permission
chmod +x pspy64

# Run pspy64
./pspy64

⚠️ Legal Disclaimer
These tools are intended for educational and ethical testing purposes only. Always ensure you have explicit permission before using these scripts on any system.

📚 Conclusion
The tools included in this repository are invaluable for penetration testers and security auditors when assessing a Linux system for potential privilege escalation vulnerabilities. Use them responsibly and follow ethical guidelines while conducting any security assessments.

