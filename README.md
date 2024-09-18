# Linux Privilege Escalation Tools

## Overview

This repository contains a collection of scripts and tools for Linux privilege escalation enumeration and analysis. Below are detailed descriptions of each tool, their purpose, usage, and how to interpret the results. The tools covered are:

1. **linpeas.sh**
2. **les.sh**
3. **LinEnum**
4. **linuxprivchecker.py**
5. **pspy64**

---

## Table of Contents

- [linpeas.sh](#linpeassh)
- [les.sh](#lessh)
- [LinEnum](#linenum)
- [linuxprivchecker.py](#linuxprivcheckerpy)
- [pspy64](#pspy64)

---

## linpeas.sh

### Description
`linpeas.sh` is a powerful script designed to check various security misconfigurations and potential privilege escalation vectors on Linux systems.

### Features
- Extensive system enumeration.
- Detects potential misconfigurations for privilege escalation.
- Identifies possible ways to gain root access through vulnerable services or file permissions.

### Usage
```bash
# Download linpeas.sh
curl -Lo linpeas.sh https://github.com/carlospolop/PEASS-ng/releases/download/refs/tags/20230918-linpeas-ng-release/linpeas.sh

# Give execution permission
chmod +x linpeas.sh

# Run linpeas.sh
./linpeas.sh

