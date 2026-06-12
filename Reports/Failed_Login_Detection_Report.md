# Failed Login Detection Report

## Objective

Detect failed authentication attempts on a Windows endpoint using Wazuh.

## Environment

- Wazuh Server: Ubuntu 24.04
- Endpoint: Windows 10
- Monitoring Tool: Wazuh SIEM

## Test Procedure

1. Installed and configured Wazuh Agent on Windows 10.
2. Generated failed login attempts using invalid credentials.
3. Monitored security events in the Wazuh Dashboard.

## Detection

### Alert Information

- Rule ID: 60122
- Severity Level: 5
- Description: Logon failure – Unknown user or bad password

### MITRE ATT&CK Mapping

- Technique: T1110 – Brute Force

## Evidence

- 10_failed_login_simulation.png
- 11_logon_failure_alerts_table.png
- 12_rule60122_alert_details.png

## Outcome

Wazuh successfully detected and generated alerts for failed authentication attempts on the Windows endpoint.