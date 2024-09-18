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

Kernel vulnerabilities.
Insecure file permissions.
SUID binaries.
Writable directories and much more.
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

