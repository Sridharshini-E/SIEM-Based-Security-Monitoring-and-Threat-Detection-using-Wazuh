# File Integrity Monitoring Report

## Objective

Monitor file creation, modification, and deletion activities using Wazuh File Integrity Monitoring (FIM).

## Environment

- Wazuh Server: Ubuntu 24.04
- Endpoint: Windows 10
- Monitored Directory: C:\SOC-Test

## Test Procedure

1. Enabled File Integrity Monitoring.
2. Added the directory C:\SOC-Test to monitoring.
3. Created test files.
4. Modified test files.
5. Deleted test files.

## Detection

### Rule IDs

- Rule 554 – File Added
- Rule 550 – Integrity Checksum Changed
- Rule 553 – File Deleted

## Evidence

- 13_fim_setup_powershell.png
- 06_fim_alerts_file_deleted.png
- 07_fim_event_detail_sha256.png

## Outcome

Wazuh successfully detected file system changes and generated alerts for file creation, modification, and deletion activities.