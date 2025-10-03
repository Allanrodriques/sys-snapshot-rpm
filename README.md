# 📋 sys-snapshot

`sys-snapshot` is a lightweight **server health snapshot tool** for **RHEL 8/9 and CentOS 8/Stream**.  
It collects critical system information and generates a **Markdown report**, useful before **migrations, audits, or troubleshooting**.

---

## 🚀 Features

- 🖥️ **System details** (hostname, kernel, OS version, uptime)  
- 🔒 **SELinux status & GRUB config**  
- ⚙️ **CPU, memory, swap usage**  
- 💾 **Disk usage, inode usage, /etc/fstab**  
- 📂 **LVM info (VGs, LVs)**  
- 📂 **NFS exports (/etc/exports)**  
- 📡 **Network interfaces, routing table, active connections, DNS config**  
- 🔥 **Firewall (firewalld + iptables)**  
- ⏰ **Cron jobs**  
- 🟢 **Active services**  
- 🔑 **Sudoers configuration**  
- 📦 **Installed packages (count + sample list)**  
- 🕒 **Timestamped reports** stored under `/var/tmp/sys-snapshot/`  

---

## 📦 Installation
1. **Download the RPM**  
   ```bash
   wget https://github.com/Allanrodriques/sys-snapshot-rpm/releases/download/v1.0/sys-snapshot-1.0-1.el8.noarch.rpm
   
2. **Import GPG key (optional, if signed)**
   ```bash
   sudo rpm --import RPM-GPG-KEY-sys-snapshot

3. **Install the package**
   ```bash
   sudo rpm -ivh sys-snapshot-1.0-1.el8.noarch.rpm


## Usage
**Run:**
sudo sys-snapshot
**Reports will be stored in:**
/var/tmp/sys-snapshot/server_health_<timestamp>.md
Example:
/var/tmp/sys-snapshot/server_health_2025-10-03_22-50-01.md








