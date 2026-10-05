# Lab 2: System Audit Automation with Bash Scripting

## Lab Objectives
- Create and structure an executable Bash script (`.sh`).
- Use native Linux commands to monitor key system resources.
- Apply output redirection (`>`) to generate automated text reports.

## Script Structure and Functionality (`audit.sh`)

The script automatically collects essential system metrics using the following logic:

1. **Shebang Interpreter (`#!/bin/bash`):** Defines the Bash execution environment.
2. **Dynamic Date Capture (`FECHA=$(date)`):** Saves the exact timestamp of the audit.
3. **Identity Audit (`whoami`):** Verifies the user executing the task.
4. **Disk Storage (`df -h /`):** Analyzes the capacity and usage percentage of the system root.
5. **RAM Status (`free -h`):** Monitors current main memory usage.

## Execution Commands

```bash
# Assign execution permissions to the script
chmod +x audit.sh

# Execution in the console
./audit.sh

# Direct export to a text report
./audit.sh > informe_sistema.txt
