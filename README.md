# Open Source Audit Project - Git

## Student Information
| Field | Details |
|-------|---------|
| **Name** | Sonal Yadav |
| **Roll Number** | 24BAI10361|
| **Slot** | A11 |
| **Course** | Open Source Software |
| **Date of Submission** | 30/03/2026 |

## Chosen Software
**Git** - A distributed version control system created by Linus Torvalds in 2005. Git is designed for speed, data integrity, and distributed non-linear workflows, making it the most widely used version control system in modern software development.

---

## Script Descriptions

| Script | Filename | Description |
|--------|----------|-------------|
| **Script 1** | `script1_system_identity.sh` | Displays a welcome screen with Linux system information including distribution name, kernel version, logged-in user, home directory, system uptime, current date/time, and the open-source license covering the OS. |
| **Script 2** | `script2_package_inspector.sh` | Checks whether Git is installed on the system, retrieves its version and license information, and uses a case statement to display a philosophical description of the software. |
| **Script 3** | `script3_disk_auditor.sh` | Loops through important system directories (/etc, /var/log, /home, /usr/bin, /tmp) and reports disk usage, ownership, and permissions for each directory. |
| **Script 4** | `script4_log_analyzer.sh` | Reads a log file line by line, counts occurrences of keywords (ERROR, WARNING, INFO), displays a summary, and shows the last 5 matching lines for the specified keyword. |
| **Script 5** | `script5_manifesto_generator.sh` | Interactively asks the user three questions about open-source philosophy and generates a personalized manifesto saved as a timestamped .txt file. |

---

## Dependencies

### System Requirements
- Linux operating system (Ubuntu/Debian, CentOS/RHEL, or Fedora)
- Bash shell (version 4.0 or higher)
- Minimum 512MB RAM
- Basic read/write permissions in the script directory

### Required Commands
All scripts use standard Linux commands that come pre-installed on most distributions:
- `bash`, `echo`, `date`, `uname`, `whoami`, `uptime`
- `dpkg` or `rpm` (for package inspection)
- `du`, `ls`, `awk`, `cut`, `grep`
- Standard file permissions (read access to log files for Script 4)

STEP BY STEP INSTRUCTIONS
1. Clone or Download the Repository
bash
git clone https://github.com/sonal-yadav02/OSS-audit--24BAI10361-.git
cd OSS-audit-24BAI10361
2. Make All Scripts Executable
bash
chmod +x *.sh
3. Run Script 1 - System Identity Report
bash
./script1_system_identity.sh
Expected Output: Displays Linux distribution, kernel version, user, home directory, uptime, date/time, and GPL license information.

4. Run Script 2 - FOSS Package Inspector
bash
./script2_package_inspector.sh
Expected Output: Shows whether Git is installed, its version number, license, and a philosophical description of the software.

5. Run Script 3 - Disk and Permission Auditor
bash
./script3_disk_auditor.sh
Expected Output: A formatted table showing directory paths, permissions with owner, and disk usage for /etc, /var/log, /home, /usr/bin, /tmp, plus Git configuration file details.

6. Run Script 4 - Log File Analyzer
bash
# Basic usage (default keyword: error)
./script4_log_analyzer.sh /var/log/syslog

# With custom keyword
./script4_log_analyzer.sh /var/log/auth.log warning
Expected Output: Total lines analyzed, counts of ERROR, WARNING, INFO keywords, and the last 5 lines containing the specified keyword.

