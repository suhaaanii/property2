# sysopctl: A Custom Linux System Administration Command

## Overview
`sysopctl` is a powerful and versatile Bash script designed to simplify Linux system administration. It integrates essential system resource management tasks into a single command-line tool. From managing services to monitoring processes and analyzing logs, `sysopctl` provides a user-friendly interface for efficient system management.

---

## Features
### Basic Features
- **Help Menu**: Displays usage instructions and available commands.
- **Version Information**: Outputs the current version of the script.

### System Management Operations
#### Easy Level
- **List Running Services**: Lists all active services on the system.
- **View System Load**: Displays system load averages.

#### Intermediate Level
- **Manage System Services**:
  - Start a specific service.
  - Stop a specific service.
- **Check Disk Usage**: Displays disk usage statistics by partition.

#### Advanced Level
- **Monitor System Processes**: Provides real-time process activity, akin to `top`.
- **Analyze System Logs**: Summarizes recent critical log entries using `journalctl`.
- **Backup System Files**: Backs up specified files or directories using `rsync`.

---

## Installation
1. **Clone the Repository**:
   ```bash
   git clone <repository_url>
   cd <repository_directory>
   ```
2. **Make the Script Executable**:
   ```bash
   chmod +x sysopctl
   ```
3. **Move to a Directory in PATH**:
   ```bash
   sudo mv sysopctl /usr/local/bin/
   ```
4. **Verify Installation**:
   ```bash
   sysopctl --version
   ```

---

## Usage
Run the command with the appropriate options as described below.

### General Commands
- **Display Help**:
  ```bash
  sysopctl --help
  ```
- **Show Version**:
  ```bash
  sysopctl --version
  ```

### Service Management
- **List Active Services**:
  ```bash
  sysopctl service list
  ```
- **Start a Service**:
  ```bash
  sysopctl service start <service-name>
  ```
- **Stop a Service**:
  ```bash
  sysopctl service stop <service-name>
  ```

### System Load
- **View System Load Averages**:
  ```bash
  sysopctl system load
  ```

### Disk Usage
- **Check Disk Usage Statistics**:
  ```bash
  sysopctl disk usage
  ```

### Process Monitoring
- **Monitor Real-Time Processes**:
  ```bash
  sysopctl process monitor
  ```

### Log Analysis
- **Analyze Critical Log Entries**:
  ```bash
  sysopctl logs analyze
  ```

### Backup Files
- **Backup a Directory or File**:
  ```bash
  sysopctl backup <path>
  ```

---

## Documentation
- **Workflow Diagrams**:
  - Refer to the `docs/diagrams` folder for workflow and system architecture visuals created using Draw.io.
- **Manual Page**:
  - A detailed manual page is included in the `docs/man` folder for integration with the `man` command. Install it as follows:
    ```bash
    sudo cp docs/man/sysopctl.1 /usr/share/man/man1/
    man sysopctl
    ```

---

## Version Control
All code and documentation are maintained in a private Git repository. Use the following commands for version control:
- **Clone the Repository**:
  ```bash
  git clone <repository_url>
  ```
- **Commit Changes**:
  ```bash
  git add .
  git commit -m "<message>"
  git push
  ```

---

## Confidentiality
This script and associated documentation are confidential and must not be shared outside of authorized personnel. Ensure proper access controls are in place for the repository.

---

## Troubleshooting
### Common Issues
1. **Command Not Found**:
   - Ensure the script is in a directory included in your `PATH`.
2. **Permission Denied**:
   - Verify the script has execute permissions: `chmod +x sysopctl`.
3. **Service Commands Fail**:
   - Use `sudo` for commands requiring elevated privileges.

